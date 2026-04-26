<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>WiFi+Bel 3Gang</title>
    <style>
        /* ===== LIGHT MODE (Mặc định) ===== */
        :root {
            --bg: #f0f2f5;
            --surface: #ffffff;
            --surface-hover: #f5f6f8;
            --text: #1a1a2e;
            --text-dim: #8888aa;
            --text-secondary: #666;
            --border: rgba(0,0,0,0.06);
            --shadow: 0 2px 12px rgba(0,0,0,0.06);
            --shadow-lg: 0 8px 30px rgba(0,0,0,0.1);
            --on: #00cc66;
            --off: #ff4444;
            --accent: #6c5ce7;
            --accent-light: rgba(108,92,231,0.1);
            --toggle-bg: #ddd;
            --card-icon-bg: #f0f0f5;
        }

        /* ===== DARK MODE ===== */
        .dark {
            --bg: #0d0d1a;
            --surface: #141428;
            --surface-hover: #1a1a36;
            --text: #e0e0e0;
            --text-dim: #606080;
            --text-secondary: #888;
            --border: rgba(255,255,255,0.05);
            --shadow: 0 2px 12px rgba(0,0,0,0.3);
            --shadow-lg: 0 8px 30px rgba(0,0,0,0.5);
            --on: #00d2a0;
            --off: #ff4757;
            --accent: #7c6cf0;
            --accent-light: rgba(108,92,231,0.15);
            --toggle-bg: #2a2a44;
            --card-icon-bg: #1a1a36;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: var(--bg);
            color: var(--text);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            padding: 20px 16px;
            transition: all 0.3s ease;
            -webkit-tap-highlight-color: transparent;
            user-select: none;
        }
        .container {
            width: 100%;
            max-width: 420px;
            display: flex;
            flex-direction: column;
            gap: 18px;
        }

        /* ===== TOP BAR ===== */
        .topbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .brand {
            font-size: 22px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }
        .brand span { color: var(--accent); }
        .top-actions {
            display: flex;
            gap: 8px;
        }
        .icon-btn {
            width: 38px; height: 38px;
            border-radius: 50%;
            background: var(--surface);
            border: 1px solid var(--border);
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 16px;
            transition: 0.3s;
            box-shadow: var(--shadow);
        }
        .icon-btn:hover { background: var(--surface-hover); }
        .icon-btn:active { transform: scale(0.92); }

        /* ===== STATUS BAR ===== */
        .status-bar {
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 10px 14px;
            background: var(--surface);
            border-radius: 14px;
            border: 1px solid var(--border);
            font-size: 12px;
            color: var(--text-dim);
            box-shadow: var(--shadow);
            transition: 0.3s;
        }
        .status-dot {
            width: 8px; height: 8px;
            border-radius: 50%;
            background: #ccc;
            animation: pulse 2s infinite;
        }
        .status-dot.connected { background: var(--on); }
        .status-dot.disconnected { background: #ff9800; animation: none; }
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.3; }
        }

        /* ===== POWER BUTTON ===== */
        .power-section {
            display: flex;
            justify-content: center;
            margin: 4px 0;
        }
        .power-btn {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            background: var(--surface);
            border: 2px solid var(--border);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: var(--shadow-lg);
            gap: 4px;
        }
        .power-btn:active { transform: scale(0.93); }
        .power-btn.all-on {
            border-color: var(--on);
            background: rgba(0,210,160,0.08);
            box-shadow: 0 0 50px rgba(0,210,160,0.2), var(--shadow-lg);
        }
        .power-btn .power-label {
            font-size: 12px;
            font-weight: 700;
            color: var(--text-dim);
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        .power-btn.all-on .power-label { color: var(--on); }
        .power-btn .power-emoji { font-size: 36px; }

        /* ===== DEVICE CARDS ===== */
        .devices {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        .device-card {
            display: flex;
            align-items: center;
            gap: 14px;
            background: var(--surface);
            border-radius: 16px;
            padding: 14px 16px;
            cursor: pointer;
            transition: all 0.3s;
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }
        .device-card:active { transform: scale(0.98); }
        .device-card.active {
            border-color: rgba(0,210,160,0.3);
            background: rgba(0,210,160,0.03);
        }
        .device-icon {
            width: 46px; height: 46px;
            border-radius: 14px;
            background: var(--card-icon-bg);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 22px;
            transition: 0.3s;
        }
        .device-card.active .device-icon {
            background: rgba(0,210,160,0.12);
        }
        .device-info { flex: 1; }
        .device-name {
            font-size: 14px;
            font-weight: 600;
            color: var(--text);
            letter-spacing: 0.3px;
        }
        .device-meta {
            font-size: 11px;
            color: var(--text-dim);
            margin-top: 2px;
            display: flex;
            align-items: center;
            gap: 6px;
        }
        .device-meta .timer-tag {
            background: rgba(255,152,0,0.12);
            color: #ff9800;
            padding: 2px 8px;
            border-radius: 8px;
            font-size: 10px;
            font-weight: 500;
        }
        .device-toggle {
            width: 50px; height: 28px;
            border-radius: 14px;
            background: var(--toggle-bg);
            cursor: pointer;
            position: relative;
            transition: 0.3s;
            flex-shrink: 0;
        }
        .device-toggle.active { background: var(--on); }
        .device-toggle::after {
            content: '';
            position: absolute;
            top: 3px; left: 3px;
            width: 22px; height: 22px;
            border-radius: 50%;
            background: #fff;
            transition: 0.3s;
            box-shadow: 0 1px 3px rgba(0,0,0,0.2);
        }
        .device-toggle.active::after { left: 25px; }

        /* ===== TIMER SECTION ===== */
        .section-label {
            font-size: 11px;
            color: var(--text-dim);
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        .timer-card {
            background: var(--surface);
            border-radius: 16px;
            padding: 14px;
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }
        .timer-row {
            display: flex;
            gap: 6px;
            margin-bottom: 8px;
            flex-wrap: wrap;
        }
        .timer-chip {
            flex: 1;
            min-width: 50px;
            padding: 9px 8px;
            border-radius: 10px;
            text-align: center;
            font-size: 12px;
            cursor: pointer;
            transition: 0.2s;
            font-weight: 500;
            background: var(--surface-hover);
            color: var(--text-dim);
            border: 1px solid var(--border);
        }
        .timer-chip.selected {
            background: var(--accent-light);
            color: var(--accent);
            border-color: var(--accent);
            font-weight: 600;
        }
        .timer-apply {
            width: 100%;
            padding: 11px;
            background: var(--accent);
            border: none;
            border-radius: 12px;
            color: #fff;
            font-weight: 600;
            font-size: 13px;
            cursor: pointer;
            letter-spacing: 0.5px;
            transition: 0.2s;
        }
        .timer-apply:active { opacity: 0.8; }

        /* ===== SETTING CARD ===== */
        .setting-card {
            background: var(--surface);
            border-radius: 16px;
            padding: 14px 16px;
            border: 1px solid var(--border);
            cursor: pointer;
            transition: 0.3s;
            box-shadow: var(--shadow);
            text-align: center;
            color: var(--text-dim);
            font-size: 14px;
            font-weight: 500;
            letter-spacing: 0.5px;
        }
        .setting-card:hover {
            border-color: var(--accent);
            color: var(--accent);
        }

        /* ===== MODE INDICATOR ===== */
        .mode-badge {
            display: inline-block;
            padding: 4px 10px;
            border-radius: 20px;
            font-size: 10px;
            font-weight: 600;
            letter-spacing: 0.5px;
        }
        .mode-ap {
            background: rgba(255,152,0,0.12);
            color: #ff9800;
        }
        .mode-sta {
            background: rgba(0,210,160,0.12);
            color: var(--on);
        }

        /* Toast */
        .toast {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            padding: 12px 22px;
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: 30px;
            color: var(--text);
            font-size: 13px;
            font-weight: 500;
            z-index: 999;
            opacity: 0;
            transition: 0.4s;
            pointer-events: none;
            box-shadow: var(--shadow-lg);
        }
        .toast.show { opacity: 1; }

        @media (max-width: 370px) {
            .device-name { font-size: 13px; }
            .power-btn { width: 110px; height: 110px; }
            .power-btn .power-emoji { font-size: 28px; }
        }
    </style>
</head>
<body>
    <div class="toast" id="toast"></div>

    <div class="container">
        <!-- TOP BAR -->
        <div class="topbar">
            <div class="brand">WiFi+Bel <span>3Gang</span></div>
            <div class="top-actions">
                <div class="icon-btn" onclick="toggleTheme()" title="Đổi giao diện">🌓</div>
                <div class="icon-btn" onclick="openSettings()" title="Cài đặt">⚙️</div>
            </div>
        </div>

        <!-- STATUS BAR -->
        <div class="status-bar" id="statusBar">
            <div class="status-dot" id="statusDot"></div>
            <span id="statusText">Đang kết nối...</span>
            <span style="flex:1"></span>
            <span class="mode-badge" id="modeBadge">AP</span>
        </div>

        <!-- POWER BUTTON -->
        <div class="power-section">
            <div class="power-btn" id="powerBtn" onclick="toggleAll()">
                <span class="power-label" id="powerLabel">ALL OFF</span>
                <span class="power-emoji">⚡</span>
            </div>
        </div>

        <!-- DEVICE LIST -->
        <div class="devices" id="deviceList"></div>

        <!-- TIMER -->
        <div class="section-label">⏱ Hẹn giờ</div>
        <div class="timer-card">
            <div style="font-size:11px;color:var(--text-dim);margin-bottom:6px">Thiết bị:</div>
            <div class="timer-row" id="timerDevices"></div>
            <div style="font-size:11px;color:var(--text-dim);margin:10px 0 6px">Thời gian:</div>
            <div class="timer-row" id="timerMinutes"></div>
            <button class="timer-apply" onclick="applyTimer()">✅ Áp dụng hẹn giờ</button>
        </div>

        <!-- SETTING -->
        <div class="section-label">⚙️ Cài đặt</div>
        <div class="setting-card" onclick="openSettings()">
            Cấu hình WiFi & Cài đặt hệ thống
        </div>
    </div>

    <script>
        // ===== CONFIG =====
        const USE_REAL_ESP = false;
        const ESP_URL = 'http://192.168.4.1';
        const names = ['Đèn', 'Quạt', 'Switch 3'];
        const icons = ['💡', '🌀', '🔌'];
        const timerOptions = [1, 5, 15, 30, 60, 120];

        let states = [false, false, false];
        let timers = {};
        let selectedTimerDevice = 0;
        let selectedTimerMin = 15;
        let darkMode = false;
        let isAPMode = true;
        let connected = false;

        // ===== THEME =====
        function toggleTheme() {
            darkMode = !darkMode;
            document.body.classList.toggle('dark', darkMode);
            localStorage.setItem('theme', darkMode ? 'dark' : 'light');
            toast(darkMode ? '🌙 Dark mode' : '☀️ Light mode');
        }

        // Load theme
        if (localStorage.getItem('theme') === 'dark') {
            darkMode = true;
            document.body.classList.add('dark');
        }

        // ===== RENDER =====
        function renderDevices() {
            let html = '';
            for (let i = 0; i < 3; i++) {
                const active = states[i];
                const hasTimer = timers[i] && timers[i] > 0;
                html += `
                <div class="device-card${active ? ' active' : ''}" onclick="toggle(${i})">
                    <div class="device-icon">${icons[i]}</div>
                    <div class="device-info">
                        <div class="device-name">${names[i]}</div>
                        <div class="device-meta">
                            <span>${active ? '🟢 Đang bật' : '⚫ Đã tắt'}</span>
                            ${hasTimer ? '<span class="timer-tag">⏱ ' + formatTime(timers[i]) + '</span>' : ''}
                        </div>
                    </div>
                    <div class="device-toggle${active ? ' active' : ''}" onclick="event.stopPropagation();toggle(${i})"></div>
                </div>`;
            }
            document.getElementById('deviceList').innerHTML = html;
        }

        function renderTimerSelects() {
            // Devices
            let dhtml = '';
            for (let i = 0; i < 3; i++) {
                dhtml += `<div class="timer-chip${selectedTimerDevice === i ? ' selected' : ''}" onclick="selectTimerDevice(${i})">${icons[i]} ${names[i]}</div>`;
            }
            document.getElementById('timerDevices').innerHTML = dhtml;

            // Minutes
            let mhtml = '';
            timerOptions.forEach(m => {
                const label = m >= 60 ? (m/60) + ' giờ' : m + ' phút';
                mhtml += `<div class="timer-chip${selectedTimerMin === m ? ' selected' : ''}" onclick="selectTimerMin(${m})">${label}</div>`;
            });
            document.getElementById('timerMinutes').innerHTML = mhtml;
        }

        function updatePowerBtn() {
            const allOn = states.every(s => s);
            const anyOn = states.some(s => s);
            const btn = document.getElementById('powerBtn');
            const label = document.getElementById('powerLabel');
            
            btn.classList.toggle('all-on', allOn);
            if (allOn) label.textContent = 'ALL ON';
            else if (anyOn) label.textContent = 'MIXED';
            else label.textContent = 'ALL OFF';
        }

        function updateStatusBar() {
            const dot = document.getElementById('statusDot');
            const text = document.getElementById('statusText');
            const badge = document.getElementById('modeBadge');
            
            if (isAPMode) {
                dot.className = 'status-dot';
                text.textContent = '📡 AP Mode: ESP32-S3-SmartSwitch';
                badge.textContent = 'AP';
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
