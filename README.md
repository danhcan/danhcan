                badge.className = 'mode-badge mode-ap';
            } else if (connected) {
                dot.className = 'status-dot connected';
                text.textContent = '✅ Đã kết nối WiFi';
                badge.textContent = 'STA';
                badge.className = 'mode-badge mode-sta';
            } else {
                dot.className = 'status-dot disconnected';
                text.textContent = '🔄 Đang kết nối...';
                badge.textContent = 'STA';
                badge.className = 'mode-badge mode-ap';
            }
        }

        function formatTime(sec) {
            if (sec >= 3600) {
                const h = Math.floor(sec/3600);
                const m = Math.floor((sec%3600)/60);
                return h + 'h' + (m > 0 ? ' ' + m + 'm' : '');
            }
            return Math.ceil(sec/60) + 'm';
        }

        function refreshUI() {
            renderDevices();
            renderTimerSelects();
            updatePowerBtn();
            updateStatusBar();
        }

        function toast(msg) {
            const t = document.getElementById('toast');
            t.textContent = msg;
            t.classList.add('show');
            clearTimeout(t._timeout);
            t._timeout = setTimeout(() => t.classList.remove('show'), 2200);
        }

        // ===== ACTIONS =====
        function toggle(id) {
            states[id] = !states[id];
            if (!states[id]) delete timers[id];
            toast((states[id] ? '🟢 Bật ' : '🔴 Tắt ') + names[id]);
            refreshUI();
        }

        function toggleAll() {
            const allOn = states.every(s => s);
            if (allOn) { states = [false, false, false]; timers = {}; toast('🔴 Tất cả đã tắt'); }
            else { states = [true, true, true]; timers = {}; toast('🟢 Tất cả đã bật'); }
            refreshUI();
        }

        function selectTimerDevice(id) { selectedTimerDevice = id; renderTimerSelects(); }
        function selectTimerMin(m) { selectedTimerMin = m; renderTimerSelects(); }

        function applyTimer() {
            states[selectedTimerDevice] = true;
            timers[selectedTimerDevice] = selectedTimerMin * 60;
            const label = selectedTimerMin >= 60 ? (selectedTimerMin/60) + 'h' : selectedTimerMin + 'm';
            toast('⏱ ' + names[selectedTimerDevice] + ' sẽ tắt sau ' + label);
            refreshUI();
        }

        function openSettings() {
            if (USE_REAL_ESP) window.location.href = ESP_URL + '/settings';
            else toast('⚙️ Cài đặt WiFi (mô phỏng)');
        }

        // ===== SIMULATE =====
        function simulateConnection() {
            isAPMode = false;
            connected = true;
            updateStatusBar();
            toast('✅ Đã kết nối WiFi nhà! AP đã tắt');
        }

        // Cho phép test chuyển mode
        setTimeout(() => {
            if (!USE_REAL_ESP) simulateConnection();
        }, 3000);

        // ===== START =====
        refreshUI();
    </script>
</body>
</html>
