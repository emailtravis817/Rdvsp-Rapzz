<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rdvsp Rapzz Dashboard</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Share+Tech+Mono&display=swap');

        :root {
            --primary-purple: #a020f0;
            --hacker-green: #00ff41;
            --dark-bg: #050505;
            --error-red: #ff003c;
        }

        body {
            background-color: var(--dark-bg);
            color: #fff;
            font-family: 'Share Tech Mono', monospace;
            display: flex;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            overflow: hidden;
        }

        /* --- MATRIX BACKGROUND --- */
        #matrix {
            position: fixed;
            top: 0; left: 0;
            z-index: -1;
            opacity: 0.2;
        }

        /* --- CONSOLE LOG LOADER --- */
        #attack-loader {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: #000;
            z-index: 1500;
            padding: 30px;
            box-sizing: border-box;
            color: var(--hacker-green);
            font-size: 14px;
            overflow: hidden;
        }

        /* --- SUCCESS OVERLAY (GLITCH EFFECT) --- */
        #success-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle, rgba(10,10,10,1) 0%, rgba(0,0,0,1) 100%);
            z-index: 1600;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            border: 4px solid var(--hacker-green);
            box-sizing: border-box;
        }

        .glitch-wrapper {
            text-align: center;
            position: relative;
        }

        .success-text {
            color: var(--hacker-green);
            font-size: 60px;
            font-weight: bold;
            letter-spacing: 15px;
            position: relative;
            text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
                        -0.025em -0.05em 0 rgba(0, 255, 0, 0.75),
                        0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
            animation: glitch 500ms infinite;
        }

        @keyframes glitch {
            0% { text-shadow: 2px 3px 0 red, -2px -3px 0 blue; transform: translate(0); }
            20% { text-shadow: -2px -3px 0 red, 2px 3px 0 blue; transform: translate(-2px, 2px); }
            40% { text-shadow: 2px -3px 0 red, -2px 3px 0 blue; transform: translate(-2px, -2px); }
            60% { text-shadow: -2px 3px 0 red, 2px -3px 0 blue; transform: translate(2px, 2px); }
            80% { text-shadow: 2px 3px 0 red, -2px -3px 0 blue; transform: translate(2px, -2px); }
            100% { text-shadow: -2px -3px 0 red, 2px 3px 0 blue; transform: translate(0); }
        }

        .system-compromised {
            color: white;
            font-size: 12px;
            margin-top: 10px;
            letter-spacing: 3px;
            opacity: 0.8;
            background: var(--hacker-green);
            color: black;
            padding: 2px 10px;
        }

        /* --- SPLASH SCREEN --- */
        #splash-screen {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: var(--dark-bg);
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            z-index: 2000;
        }

        .logo-splash { font-family: 'Pacifico', cursive; font-size: 40px; text-shadow: 0 0 20px var(--primary-purple); }

        /* --- DASHBOARD UI --- */
        .container { width: 90%; max-width: 400px; padding: 20px; padding-bottom: 100px; display: none; }
        .profile-card { background: rgba(20, 20, 20, 0.9); border: 1px solid var(--primary-purple); padding: 25px 20px; border-radius: 15px; text-align: center; box-shadow: 0 0 20px rgba(160, 32, 240, 0.4); margin-bottom: 20px; }
        .rapzz-hacker-text { font-family: 'Pacifico', cursive; font-size: 30px; text-shadow: 0 0 10px var(--primary-purple); }
        .profile-info { font-size: 13px; margin-top: 10px; color: var(--hacker-green); }
        #clock { font-size: 20px; color: #fff; margin-top: 5px; }

        .page { display: none; animation: fadeIn 0.5s; }
        .active-page { display: block; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .card { background: rgba(30, 30, 30, 0.9); border: 1px solid #333; border-radius: 15px; padding: 20px; margin-bottom: 15px; }
        h3 { color: var(--primary-purple); font-size: 16px; border-bottom: 1px solid #333; padding-bottom: 5px; margin-top: 0;}
        p { font-size: 13px; color: #ccc; line-height: 1.4; }

        input, select { width: 100%; background: #000; border: 1px solid #444; border-radius: 8px; padding: 12px; color: var(--hacker-green); margin-bottom: 15px; font-family: inherit; }
        .btn { width: 100%; background: var(--primary-purple); color: white; border: none; padding: 15px; border-radius: 10px; cursor: pointer; font-weight: bold; text-transform: uppercase; box-shadow: 0 0 10px var(--primary-purple); }

        .tool-item { border: 1px solid #444; padding: 15px; margin-bottom: 10px; border-radius: 10px; text-align: center; background: rgba(0,0,0,0.5); cursor: pointer; color: var(--hacker-green); }

        .bottom-nav { position: fixed; bottom: 15px; width: 90%; max-width: 380px; background: rgba(10, 10, 10, 0.95); display: flex; justify-content: space-around; padding: 12px 0; border-radius: 20px; border: 1px solid #333; }
        .nav-item { text-decoration: none; text-align: center; font-size: 18px; color: var(--hacker-green); transition: 0.3s; }
        .nav-item.active { color: var(--primary-purple); text-shadow: 0 0 10px var(--primary-purple); }
        .nav-label { display: block; font-size: 10px; margin-top: 3px; }
    </style>
</head>
<body onload="initSite()">

<div id="splash-screen">
    <div class="logo-splash">𝙍𝙙𝙫𝙨𝙥 𝙍𝗮𝗽𝘇𝘇</div>
    <div style="color: var(--primary-purple); margin-top: 10px; font-size: 12px;">BYPASSING ENCRYPTION...</div>
</div>

<canvas id="matrix"></canvas>

<div id="attack-loader">
    <div id="console-logs"></div>
</div>

<div id="success-overlay">
    <div class="glitch-wrapper">
        <div class="success-text" data-text="SUCCESS">SUCCESS</div>
        <div class="system-compromised">SYSTEM BREACHED - ACCESS GRANTED</div>
    </div>
    <button class="btn" style="width: 180px; margin-top: 50px; background: transparent; border: 1px solid var(--hacker-green); color: var(--hacker-green); box-shadow: 0 0 15px var(--hacker-green);" onclick="closeSuccess()">RETURN TO BASE</button>
</div>

<div class="container" id="main-container">
    <div class="profile-card">
        <div class="rapzz-hacker-text">𝙍𝙙𝙫𝙨𝙥 𝙍𝗮𝗽𝘇𝘇</div>
        <div class="profile-info">
            <div>SYSTEM STATUS: <span style="color:white">ONLINE</span></div>
            <div>LICENSE: PREMIUM 2026-2030</div>
            <div id="clock">00:00:00</div>
        </div>
    </div>

    <div id="main" class="page active-page">
        <div class="card">
            <h3>INFO BUG WHATSAPP</h3>
            <p>Eksploitasi celah server pesan yang dapat membekukan aplikasi target dalam hitungan detik.</p>
        </div>
        <div class="card">
            <h3>INFO CRASH ANDROID</h3>
            <p>Pengiriman paket data biner masif untuk memaksa sistem Android melakukan force close instan.</p>
        </div>
        <div class="card">
            <h3>INFO CRASH IOS</h3>
            <p>Bug rendering font pada library grafis iPhone penyebab respring sistem secara paksa.</p>
        </div>
        <div class="card">
            <h3>MEMBERSHIP PREMIUM</h3>
            <p>Dapatkan akses penuh ke tools bot otomatis dan jalur bypass nomor tanpa verifikasi.</p>
        </div>
    </div>

    <div id="bug" class="page">
        <div class="card">
            <p style="color:var(--primary-purple); margin-bottom:10px;">> ATTACK_MODULE_V1.0</p>
            <input type="tel" id="targetBug" placeholder="+62xxxxxxxxxx">
            <select id="bugType">
                <option value="BUG WHATSAPP">BUG WHATSAPP</option>
                <option value="CRASH ANDROID">CRASH ANDROID</option>
                <option value="CRASH IOS">CRASH IOS</option>
            </select>
            <button class="btn" onclick="startAttack('targetBug')">EXECUTE ATTACK</button>
        </div>
    </div>

    <div id="tools" class="page">
        <div id="tools-list">
            <p style="text-align: center; color: var(--primary-purple); margin-bottom: 10px;">Select Premium Tool</p>
            <div class="tool-item" onclick="showToolAction('BAND WHATSAPP')">BAND WHATSAPP</div>
            <div class="tool-item" onclick="showToolAction('UNBAND WHATSAPP')">UNBAND WHATSAPP</div>
            <div class="tool-item" onclick="showToolAction('BOT PO WHATSAPP')">BOT PO WHATSAPP</div>
            <div class="tool-item" onclick="showToolAction('RESET ANDROID')">RESET ANDROID</div>
            <div class="tool-item" onclick="showToolAction('RESET IOS')">RESET IOS</div>
        </div>
        <div id="tool-action" style="display: none;">
            <div class="card">
                <h3 id="selected-tool-title">TOOL NAME</h3>
                <input type="tel" id="targetTool" placeholder="+62xxxxxxxxxx">
                <button class="btn" onclick="startAttack('targetTool')">EXECUTE ATTACK</button>
                <button class="btn" style="background: #222; margin-top: 10px; box-shadow: none;" onclick="backToTools()">CANCEL</button>
            </div>
        </div>
    </div>

    <div id="chat" class="page">
        <div class="card" style="text-align:center; padding: 40px 20px;">
            <h3>ADMIN SUPPORT</h3>
            <button class="btn" onclick="window.location.href='https://wa.me/62882007235276'">CHAT DEVELOPER</button>
            <p style="margin-top:20px; font-size:11px;">𝘼𝙡𝙬𝙖𝙮𝙨 𝙪𝙨𝙚 𝙑𝙋𝙉 𝙬𝙝𝙚𝙣 𝙖𝙩𝙩𝙖𝙘𝙠𝙞𝙣𝙜.</p>
        </div>
    </div>

    <div class="bottom-nav">
        <a href="javascript:void(0)" class="nav-item active" onclick="openPage(event, 'main')">🏠<span class="nav-label">HOME</span></a>
        <a href="javascript:void(0)" class="nav-item" onclick="openPage(event, 'bug')">📡<span class="nav-label">BUG</span></a>
        <a href="javascript:void(0)" class="nav-item" onclick="openPage(event, 'tools')">⚡<span class="nav-label">TOOLS</span></a>
        <a href="javascript:void(0)" class="nav-item" onclick="openPage(event, 'chat')">💬<span class="nav-label">CHAT</span></a>
    </div>
</div>

<script>
    function initSite() {
        setTimeout(() => {
            document.getElementById('splash-screen').style.display = 'none';
            document.getElementById('main-container').style.display = 'block';
        }, 2500);
    }

    function openPage(evt, pageName) {
        var page = document.getElementsByClassName("page");
        for (var i = 0; i < page.length; i++) { page[i].classList.remove("active-page"); }
        var navlinks = document.getElementsByClassName("nav-item");
        for (var i = 0; i < navlinks.length; i++) { navlinks[i].classList.remove("active"); }
        document.getElementById(pageName).classList.add("active-page");
        evt.currentTarget.classList.add("active");
        if(pageName !== 'tools') backToTools();
    }

    function showToolAction(toolName) {
        document.getElementById('tools-list').style.display = 'none';
        document.getElementById('tool-action').style.display = 'block';
        document.getElementById('selected-tool-title').innerText = toolName;
    }

    function backToTools() {
        document.getElementById('tools-list').style.display = 'block';
        document.getElementById('tool-action').style.display = 'none';
    }

    function startAttack(inputId) {
        const num = document.getElementById(inputId).value;
        if(!num) { alert("Masukkan nomor target!"); return; }

        const loader = document.getElementById('attack-loader');
        const logs = document.getElementById('console-logs');
        loader.style.display = 'block';
        logs.innerHTML = '';
        
        const hackingSteps = [
            "[!] INITIALIZING CORE MODULES...",
            "[+] TARGET ACQUIRED: " + num,
            "[*] INJECTING SQL PAYLOAD...",
            "[*] BYPASSING OTP HANDLER...",
            "[!] EXPLOITING BUFFER OVERFLOW...",
            "[+] SERVER ROOT ACCESS GRANTED",
            "[*] SENDING CRASH PACKETS...",
            "[!] CLEARING SYSTEM LOGS...",
            "[+] SUCCESS: EXPLOIT DELIVERED!"
        ];

        let i = 0;
        const interval = setInterval(() => {
            if (i < hackingSteps.length) {
                const p = document.createElement('p');
                p.innerText = hackingSteps[i];
                p.style.margin = "5px 0";
                logs.appendChild(p);
                i++;
            } else {
                clearInterval(interval);
                setTimeout(() => {
                    loader.style.display = 'none';
                    document.getElementById('success-overlay').style.display = 'flex';
                }, 1000);
            }
        }, 500);
    }

    function closeSuccess() {
        document.getElementById('success-overlay').style.display = 'none';
        backToTools();
    }

    const canvas = document.getElementById('matrix');
    const ctx = canvas.getContext('2d');
    canvas.width = window.innerWidth; canvas.height = window.innerHeight;
    const letters = "01"; const fontSize = 16;
    const columns = canvas.width / fontSize;
    const drops = Array(Math.floor(columns)).fill(1);

    function drawMatrix() {
        ctx.fillStyle = "rgba(0, 0, 0, 0.05)"; ctx.fillRect(0, 0, canvas.width, canvas.height);
        ctx.fillStyle = "#a020f0"; ctx.font = fontSize + "px arial";
        for (let i = 0; i < drops.length; i++) {
            const text = letters[Math.floor(Math.random() * letters.length)];
            ctx.fillText(text, i * fontSize, drops[i] * fontSize);
            if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) drops[i] = 0;
            drops[i]++;
        }
    }
    setInterval(drawMatrix, 50);

    function updateClock() {
        document.getElementById('clock').textContent = new Date().toLocaleTimeString('id-ID');
    }
    setInterval(updateClock, 1000);
</script>

</body>
</html>
