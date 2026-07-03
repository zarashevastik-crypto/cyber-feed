<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CYBER FEED 4.0</title>
    <style>
        /* Базовые переменные (Темная тема) */
        :root { --bg: #0b0e14; --panel: #141923; --border: #222d3f; --accent: #00f2fe; --accent-grad: linear-gradient(135deg, #00f2fe 0%, #4facfe 100%); --text: #f4f6f9; }
        
        /* Светлая/Неоновая тема */
        body.theme-neon { --bg: #000a12; --panel: #011124; --border: #00ffcc; --accent: #00ffcc; --accent-grad: linear-gradient(135deg, #00ffcc 0%, #00ccff 100%); --text: #e0ffff; text-shadow: 0 0 2px rgba(0,255,204,0.3); }

        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background: var(--bg); color: var(--text); margin: 0; padding: 10px 15px 80px 15px; transition: background 0.3s, color 0.3s; }
        .container { max-width: 550px; margin: 0 auto; }
        
        header { display: flex; justify-content: space-between; align-items: center; padding: 10px 0; border-bottom: 1px solid var(--border); margin-bottom: 15px; }
        .logo { font-size: 22px; font-weight: 900; color: var(--accent); text-shadow: 0 0 10px var(--accent); letter-spacing: 1px; }
        
        /* Уведомления и Тема */
        .header-tools { display: flex; gap: 10px; align-items: center; }
        .theme-btn { background: var(--panel); border: 1px solid var(--border); color: var(--text); padding: 8px; border-radius: 10px; cursor: pointer; font-size: 16px; }
        .notif-bell { position: relative; cursor: pointer; font-size: 20px; background: var(--panel); padding: 8px 12px; border-radius: 10px; border: 1px solid var(--border); }
        .notif-badge { position: absolute; top: -5px; right: -5px; background: #ff4a5a; color: white; font-size: 11px; font-weight: bold; padding: 2px 6px; border-radius: 10px; display: none; }

        .nav-tabs { display: flex; gap: 8px; margin-bottom: 15px; }
        .tab-btn { flex: 1; background: var(--panel); border: 1px solid var(--border); color: #8aa0c2; padding: 10px; border-radius: 10px; font-weight: bold; cursor: pointer; text-align: center; transition: 0.2s; }
        .tab-btn.active { background: var(--accent-grad); color: #000; border-color: transparent; }

        /* Экран авторизации */
        #authModal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: var(--bg); z-index: 1000; display: flex; justify-content: center; align-items: center; padding: 20px; box-sizing: border-box; }
        .auth-box { background: var(--panel); border: 2px solid var(--accent); padding: 25px; border-radius: 16px; width: 100%; max-width: 380px; text-align: center; box-shadow: 0 0 30px rgba(0,242,254,0.1); }
        
        input, textarea, select { width: 100%; background: rgba(0,0,0,0.2); border: 1px solid var(--border); border-radius: 8px; color: var(--text); padding: 12px; font-size: 15px; outline: none; box-sizing: border-box; margin-bottom: 10px; font-family: inherit; transition: 0.2s; }
        input:focus, textarea:focus { border-color: var(--accent); box-shadow: 0 0 8px rgba(0,242,254,0.2); }
        textarea { resize: none; height: 60px; }
        
        .main-btn { width: 100%; background: var(--accent-grad); border: none; border-radius: 8px; color: #000; padding: 12px; font-weight: 800; cursor: pointer; font-size: 15px; transition: 0.2s; }
        .main-btn:active { transform: scale(0.98); }
        
        .tools-bar { display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px; }
        .emoji-bar { display: flex; gap: 10px; font-size: 20px; user-select: none; }
        .emoji-bar span { cursor: pointer; transition: 0.1s; }
        .emoji-bar span:active { transform: scale(1.4); }
        .file-label { background: rgba(0,0,0,0.3); color: var(--accent); padding: 6px 12px; border-radius: 6px; font-size: 13px; cursor: pointer; display: flex; align-items: center; gap: 5px; font-weight: bold; border: 1px solid var(--border); }
        #previewImg { max-width: 100%; max-height: 150px; border-radius: 8px; margin-bottom: 10px; display: none; border: 1px solid var(--border); }

        .post { background: var(--panel); padding: 16px; border-radius: 14px; border: 1px solid var(--border); margin-bottom: 15px; animation: fadeIn 0.4s ease; box-shadow: 0 4px 15px rgba(0,0,0,0.2); }
        .post-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px; }
        .post-author { font-weight: bold; color: var(--accent); font-size: 15px; display: flex; align-items: center; gap: 6px; }
        .post-time { font-size: 11px; color: #627593; }
        .post-content { line-height: 1.4; font-size: 14px; word-break: break-word; margin-bottom: 10px; white-space: pre-wrap; }
        .post-image { max-width: 100%; border-radius: 10px; margin-bottom: 10px; border: 1px solid var(--border); }
        .hashtag { color: var(--accent); font-weight: bold; cursor: pointer; text-decoration: underline; }
        
        .post-actions { display: flex; gap: 8px; border-top: 1px solid rgba(255,255,255,0.05); padding-top: 10px; flex-wrap: wrap; }
        .action-btn { background: rgba(0,0,0,0.2); border: 1px solid var(--border); color: var(--text); padding: 6px 10px; border-radius: 6px; cursor: pointer; font-size: 12px; display: flex; align-items: center; gap: 5px; }
        .action-btn:hover { border-color: var(--accent); }

        .comments-section { margin-top: 10px; padding-top: 10px; border-top: 1px dashed var(--border); display: none; }
        .comment-item { font-size: 13px; background: rgba(0,0,0,0.2); padding: 8px 10px; border-radius: 6px; margin-bottom: 6px; display: flex; justify-content: space-between; align-items: center; }
        .comment-author { color: var(--accent); font-weight: bold; margin-right: 5px; }
        .del-comment { color: #ff4a5a; cursor: pointer; font-size: 14px; font-weight: bold; padding: 0 5px; }

        /* Директ и онлайн статусы */
        .dm-user-list { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 10px; margin-bottom: 15px; }
        .dm-user { background: rgba(0,0,0,0.2); padding: 8px 14px; border-radius: 20px; border: 1px solid var(--border); cursor: pointer; white-space: nowrap; font-size: 13px; position: relative; }
        .dm-user.active { border-color: var(--accent); background: var(--panel); color: var(--accent); }
        .online-dot { display: inline-block; width: 8px; height: 8px; background: #00ffcc; border-radius: 50%; margin-left: 5px; box-shadow: 0 0 5px #00ffcc; }
        .offline-dot { display: inline-block; width: 8px; height: 8px; background: #627593; border-radius: 50%; margin-left: 5px; }

        .chat-box { background: rgba(0,0,0,0.3); border: 1px solid var(--border); border-radius: 10px; height: 300px; overflow-y: auto; padding: 10px; display: flex; flex-direction: column; gap: 8px; margin-bottom: 10px; }
        .msg { max-width: 75%; padding: 8px 12px; border-radius: 10px; font-size: 13px; }
        .msg.mine { align-self: flex-end; background: var(--accent-grad); color: #000; font-weight: 500; }
        .msg.other { align-self: flex-start; background: var(--panel); color: var(--text); border: 1px solid var(--border); }

        #notifModal { display: none; background: var(--panel); border: 1px solid var(--accent); padding: 15px; border-radius: 12px; margin-bottom: 15px; box-shadow: 0 4px 20px rgba(0,0,0,0.5); }
        .notif-item { font-size: 13px; padding: 8px 0; border-bottom: 1px solid var(--border); }
        
        .hidden { display: none !important; }
        @keyframes fadeIn { from { opacity: 0; transform: scale(0.98); } to { opacity: 1; transform: scale(1); } }
    </style>
</head>
<body>

    <!-- Экран Входа -->
    <div id="authModal">
        <div class="auth-box">
            <h2 style="color: var(--accent); margin-top:0; font-weight: 900; letter-spacing: 1px;">⚡ CYBER ID</h2>
            <p style="font-size: 13px; color: #8aa0c2;">Доступ в закрытую сеть</p>
            <input type="text" id="loginNick" placeholder="Твой никнейм (например, Астемир)">
            <select id="loginAvatar">
                <option value="👑">👑 Лидер</option>
                <option value="⚡">⚡ Кибер</option>
                <option value="🤖">🤖 Хакер</option>
                <option value="🔥">🔥 Огонь</option>
                <option value="👽">👽 Пришелец</option>
            </select>
            <button class="main-btn" onclick="login()">Подключиться к узлу</button>
        </div>
    </div>

    <!-- Основной интерфейс -->
    <div class="container" id="mainApp" style="display: none;">
        <header>
            <div class="logo">⚡ CF_4.0</div>
            <div class="header-tools">
                <button class="theme-btn" onclick="toggleTheme()">🌗</button>
                <span id="currentUserDisplay" style="font-size: 14px; font-weight: bold; color: var(--accent);"></span>
                <div class="notif-bell" onclick="toggleNotifModal()">
                    🔔 <span class="notif-badge" id="notifBadge">0</span>
                </div>
            </div>
        </header>

        <div id="notifModal">
            <b style="color: var(--accent); font-size: 14px;">Системные логи:</b>
            <div id="notifList"></div>
        </div>

        <div class="nav-tabs">
            <div class="tab-btn active" id="tabFeedBtn" onclick="switchTab('feed')">📰 Лента</div>
            <div class="tab-btn" id="tabDmBtn" onclick="switchTab('dm')">💬 Директ</div>
            <div class="tab-btn" onclick="logout()" style="flex: 0.4; background: rgba(255,74,90,0.1); color: #ff4a5a; border-color: rgba(255,74,90,0.3);">🚪 Выход</div>
        </div>

        <!-- Лента -->
        <div id="tabFeed">
            <input type="text" id="searchInput" placeholder="🔍 Поиск по автору, тексту или #тегу...">

            <div style="background: var(--panel); padding: 15px; border-radius: 14px; border: 1px solid var(--border); margin-bottom: 20px; box-shadow: 0 4px 15px rgba(0,0,0,0.2);">
                <textarea id="postInput" placeholder="Что транслируем в сеть? (используй #хэштеги)"></textarea>
                <img id="previewImg">
                <div class="tools-bar">
                    <div class="emoji-bar">
                        <span onclick="pressEmoji('🔥')">🔥</span>
                        <span onclick="pressEmoji('🚀')">🚀</span>
                        <span onclick="pressEmoji('😂')">😂</span>
                        <span onclick="pressEmoji('💻')">💻</span>
                        <span onclick="pressEmoji('👽')">👽</span>
                    </div>
                    <label class="file-label">
                        📎 Файл
                        <input type="file" id="imageInput" accept="image/*" style="display: none;" onchange="handleImageUpload(event)">
                    </label>
                </div>
                <button class="main-btn" id="submitBtn" onclick="sendPost()">Опубликовать пакет</button>
            </div>

            <div id="feed"></div>
        </div>

        <!-- Директ -->
        <div id="tabDm" class="hidden">
            <div style="font-size: 13px; color: #8aa0c2; margin-bottom: 8px;">Доступные контакты:</div>
            <div class="dm-user-list" id="dmUserList"></div>
            
            <div id="chatArea" class="hidden">
                <div style="font-weight: bold; margin-bottom: 8px; color: var(--accent);" id="chatWithTitle"></div>
                <div class="chat-box" id="chatBox"></div>
                <div style="display: flex; gap: 8px;">
                    <input type="text" id="dmInput" placeholder="Шифрованное сообщение..." style="margin-bottom: 0;">
                    <button class="main-btn" style="width: 80px; padding: 0;" onclick="sendDm()">➡️</button>
                </div>
            </div>
        </div>
    </div>

    <script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-database.js"></script>

    <script>
        // Тот же конфиг Firebase
        const firebaseConfig = {
            apiKey: "AIzaSyDpVfyvm6r-KuH2xNdJSx93L12uYXjh2Bo",
            authDomain: "my-social-net.firebaseapp.com",
            databaseURL: "https://my-social-net-default-rtdb.firebaseio.com/",
            projectId: "my-social-net",
            storageBucket: "my-social-net.firebasestorage.app",
            messagingSenderId: "998951685291",
            appId: "1:998951685291:web:01a734789a711860af3bee"
        };
        firebase.initializeApp(firebaseConfig);
        const db = firebase.database();

        let currentUser = null;
        let selectedImageBase64 = null;
        let currentPostsArray = [];
        let searchQuery = "";
        let activeDmUser = null;
        let onlineUsers = {}; // Храним статусы онлайна

        // Звуки
        function playSound(type) {
            try {
                const ctx = new (window.AudioContext || window.webkitAudioContext)();
                const osc = ctx.createOscillator(); const gain = ctx.createGain();
                osc.connect(gain); gain.connect(ctx.destination);
                if (type === 'click') { osc.frequency.setValueAtTime(800, ctx.currentTime); osc.frequency.exponentialRampToValueAtTime(1100, ctx.currentTime + 0.05); gain.gain.setValueAtTime(0.1, ctx.currentTime); gain.gain.linearRampToValueAtTime(0, ctx.currentTime + 0.05); osc.start(); osc.stop(ctx.currentTime + 0.05); }
                else if (type === 'send') { osc.type = 'square'; osc.frequency.setValueAtTime(300, ctx.currentTime); osc.frequency.exponentialRampToValueAtTime(900, ctx.currentTime + 0.1); gain.gain.setValueAtTime(0.05, ctx.currentTime); gain.gain.linearRampToValueAtTime(0, ctx.currentTime + 0.1); osc.start(); osc.stop(ctx.currentTime + 0.1); }
            } catch(e) {}
        }

        // --- SPA АВТОРИЗАЦИЯ (Без перезагрузок) ---
        window.onload = () => {
            const savedNick = localStorage.getItem("cyber_nick");
            const savedAvatar = localStorage.getItem("cyber_avatar");
            const savedTheme = localStorage.getItem("cyber_theme");
            if (savedTheme === 'neon') document.body.classList.add("theme-neon");

            if (savedNick && savedAvatar) {
                currentUser = { nick: savedNick, avatar: savedAvatar };
                showMainApp();
                initApp();
            }
        };

        function login() {
            const nick = document.getElementById("loginNick").value.trim();
            const avatar = document.getElementById("loginAvatar").value;
            if (!nick) return alert("Введите позывной!");
            currentUser = { nick, avatar };
            localStorage.setItem("cyber_nick", nick);
            localStorage.setItem("cyber_avatar", avatar);
            playSound('send');
            showMainApp();
            initApp();
        }

        // ИСПРАВЛЕННЫЙ ВЫХОД
        function logout() {
            localStorage.removeItem("cyber_nick");
            localStorage.removeItem("cyber_avatar");
            
            // Отключаем статус онлайна
            if (currentUser) db.ref("users_status/" + currentUser.nick).set(false);
            
            // Жестко отключаем все слушатели от Firebase, чтобы они не кэшировались
            db.ref().off();
            
            currentUser = null;
            activeDmUser = null;
            
            // Скрываем приложение, показываем авторизацию (Без window.reload!)
            document.getElementById("mainApp").style.display = "none";
            document.getElementById("authModal").style.display = "flex";
            
            // Очищаем визуал
            document.getElementById("feed").innerHTML = "";
            document.getElementById("chatBox").innerHTML = "";
            document.getElementById("chatArea").classList.add("hidden");
            document.getElementById("notifBadge").style.display = "none";
            document.getElementById("loginNick").value = "";
        }

        function showMainApp() {
            document.getElementById("authModal").style.display = "none";
            document.getElementById("mainApp").style.display = "block";
            document.getElementById("currentUserDisplay").innerText = `${currentUser.avatar} ${currentUser.nick}`;
        }

        function toggleTheme() {
            document.body.classList.toggle("theme-neon");
            const isNeon = document.body.classList.contains("theme-neon");
            localStorage.setItem("cyber_theme", isNeon ? "neon" : "dark");
            playSound('click');
        }

        // --- ИНИЦИАЛИЗАЦИЯ ДАННЫХ ---
        function initApp() {
            // 1. Установка статуса онлайна
            const myStatusRef = db.ref("users_status/" + currentUser.nick);
            db.ref(".info/connected").on("value", (snap) => {
                if (snap.val() === true) {
                    myStatusRef.onDisconnect().set(false);
                    myStatusRef.set(true);
                }
            });

            // 2. Слушаем онлайн других пользователей
            db.ref("users_status").on("value", (snap) => {
                onlineUsers = snap.val() || {};
                updateDmListUI();
            });

            // 3. Слушаем ленту
            db.ref("posts").on("value", (snapshot) => {
                currentPostsArray = [];
                snapshot.forEach((child) => {
                    const post = child.val();
                    post.id = child.key;
                    currentPostsArray.push(post);
                });
                renderFeed();
                updateDmListUI();
            });

            // 4. Слушаем уведомления
            db.ref("notifications/" + currentUser.nick).on("value", (snapshot) => {
                const notifList = document.getElementById("notifList");
                notifList.innerHTML = "";
                let count = 0;
                snapshot.forEach((child) => {
                    count++;
                    const n = child.val();
                    notifList.innerHTML += `<div class="notif-item">🔔 <b>${n.from}</b>: ${n.text}</div>`;
                });
                const badge = document.getElementById("notifBadge");
                if (count > 0) { badge.innerText = count; badge.style.display = "inline-block"; playSound('click'); }
                else { badge.style.display = "none"; }
            });
        }

        // --- ПОСТЫ И КОММЕНТАРИИ ---
        function handleImageUpload(event) {
            const file = event.target.files[0];
            if (!file) return;
            const reader = new FileReader();
            reader.onload = function(e) {
                const img = new Image();
                img.onload = function() {
                    const canvas = document.createElement("canvas");
                    const MAX_WIDTH = 400; const scaleSize = MAX_WIDTH / img.width;
                    canvas.width = MAX_WIDTH; canvas.height = img.height * scaleSize;
                    const ctx = canvas.getContext("2d"); ctx.drawImage(img, 0, 0, canvas.width, canvas.height);
                    selectedImageBase64 = canvas.toDataURL("image/jpeg", 0.6);
                    document.getElementById("previewImg").src = selectedImageBase64;
                    document.getElementById("previewImg").style.display = "block";
                    playSound('click');
                }
                img.src = e.target.result;
            }
            reader.readAsDataURL(file);
        }

        function sendPost() {
            const text = document.getElementById("postInput").value.trim();
            if (!text && !selectedImageBase64) return alert("Пакет пуст!");
            db.ref("posts").push({
                author: currentUser.nick, avatar: currentUser.avatar, content: text,
                image: selectedImageBase64 || null, createdAt: Date.now(), likes: 0, likedBy: {}
            });
            document.getElementById("postInput").value = "";
            document.getElementById("previewImg").style.display = "none";
            selectedImageBase64 = null;
            playSound('send');
        }

        function likePost(postId, authorNick) {
            playSound('click');
            const postRef = db.ref("posts/" + postId);
            postRef.once("value", (s) => {
                const post = s.val(); let likes = post.likes || 0; let likedBy = post.likedBy || {};
                if (likedBy[currentUser.nick]) { likes--; delete likedBy[currentUser.nick]; } 
                else {
                    likes++; likedBy[currentUser.nick] = true;
                    if (authorNick !== currentUser.nick) db.ref("notifications/" + authorNick).push({ from: currentUser.nick, text: "оценил(а) ваш пост ❤️" });
                }
                postRef.update({ likes, likedBy });
            });
        }

        function toggleComments(postId) {
            const sec = document.getElementById("comments-" + postId);
            sec.style.display = sec.style.display === "block" ? "none" : "block";
        }

        function sendComment(postId, authorNick) {
            const input = document.getElementById("commInput-" + postId);
            const text = input.value.trim();
            if (!text) return;
            db.ref("posts/" + postId + "/comments").push({ author: currentUser.nick, text: text, time: Date.now() });
            if (authorNick !== currentUser.nick) db.ref("notifications/" + authorNick).push({ from: currentUser.nick, text: `коммент: "${text}"` });
            input.value = ""; playSound('send');
        }

        function deleteComment(postId, commentId) {
            if (confirm("Стереть комментарий?")) {
                db.ref("posts/" + postId + "/comments/" + commentId).remove();
            }
        }

        // --- ДИРЕКТ ---
        function updateDmListUI() {
            // Собираем уникальных юзеров из постов
            const usersSet = new Set(Object.keys(onlineUsers)); 
            currentPostsArray.forEach(p => { if (p.author && p.author !== currentUser.nick) usersSet.add(p.author); });
            usersSet.delete(currentUser.nick); // Убираем себя
            
            const list = document.getElementById("dmUserList");
            list.innerHTML = "";
            usersSet.forEach(u => {
                const isOnline = onlineUsers[u] === true;
                const dotClass = isOnline ? "online-dot" : "offline-dot";
                list.innerHTML += `<div class="dm-user ${activeDmUser === u ? 'active' : ''}" onclick="openChat('${u}')">👤 ${u} <span class="${dotClass}"></span></div>`;
            });
        }

        function openChat(targetUser) {
            activeDmUser = targetUser;
            document.getElementById("chatArea").classList.remove("hidden");
            document.getElementById("chatWithTitle").innerText = `Шифр-канал: ${targetUser}`;
            updateDmListUI();
            
            const roomId = [currentUser.nick, targetUser].sort().join("_");
            db.ref("directs/" + roomId).on("value", (s) => {
                const box = document.getElementById("chatBox");
                box.innerHTML = "";
                s.forEach(child => {
                    const m = child.val();
                    const isMine = m.from === currentUser.nick;
                    box.innerHTML += `<div class="msg ${isMine ? 'mine' : 'other'}"><b>${isMine ? 'Вы' : m.from}:</b> ${m.text}</div>`;
                });
                box.scrollTop = box.scrollHeight;
            });
        }

        function sendDm() {
            const input = document.getElementById("dmInput"); const text = input.value.trim();
            if (!text || !activeDmUser) return;
            const roomId = [currentUser.nick, activeDmUser].sort().join("_");
            db.ref("directs/" + roomId).push({ from: currentUser.nick, text: text, time: Date.now() });
            db.ref("notifications/" + activeDmUser).push({ from: currentUser.nick, text: "новое сообщение в Директ ✉️" });
            input.value = ""; playSound('send');
        }

        // --- UI УТИЛИТЫ ---
        function switchTab(tab) {
            document.getElementById("tabFeed").className = tab === 'feed' ? '' : 'hidden';
            document.getElementById("tabDm").className = tab === 'dm' ? '' : 'hidden';
            document.getElementById("tabFeedBtn").className = `tab-btn ${tab === 'feed' ? 'active' : ''}`;
            document.getElementById("tabDmBtn").className = `tab-btn ${tab === 'dm' ? 'active' : ''}`;
        }

        function toggleNotifModal() {
            const m = document.getElementById("notifModal");
            m.style.display = m.style.display === "block" ? "none" : "block";
            if (m.style.display === "block") {
                db.ref("notifications/" + currentUser.nick).remove();
                document.getElementById("notifBadge").style.display = "none";
            }
        }

        function pressEmoji(emoji) { document.getElementById("postInput").value += emoji; document.getElementById("postInput").focus(); playSound('click'); }
        function filterTag(tag) { document.getElementById("searchInput").value = tag; searchQuery = tag.toLowerCase(); renderFeed(); }
        document.getElementById("searchInput").addEventListener("input", (e) => { searchQuery = e.target.value.toLowerCase().trim(); renderFeed(); });

        function renderFeed() {
            const feedHTML = document.getElementById("feed");
            feedHTML.innerHTML = "";
            [...currentPostsArray].reverse().forEach((post) => {
                const authorNick = post.author || "Аноним"; const avatar = post.avatar || "👤";
                let contentText = post.content || "";

                if (searchQuery && !authorNick.toLowerCase().includes(searchQuery) && !contentText.toLowerCase().includes(searchQuery)) return;

                contentText = contentText.replace(/(#[а-яА-Яa-zA-Z0-9_]+)/g, `<span class="hashtag" onclick="filterTag('$1')">$1</span>`);
                const time = new Date(post.createdAt).toLocaleString('ru-RU', { hour: '2-digit', minute: '2-digit', day: '2-digit', month: '2-digit' });
                const likesCount = post.likes || 0;
                const isLiked = post.likedBy && post.likedBy[currentUser.nick];

                let commentsHTML = "";
                if (post.comments) {
                    Object.entries(post.comments).forEach(([commId, c]) => {
                        const canDelete = c.author === currentUser.nick;
                        commentsHTML += `<div class="comment-item">
                            <div><span class="comment-author">${c.author}:</span>${c.text}</div>
                            ${canDelete ? `<span class="del-comment" onclick="deleteComment('${post.id}', '${commId}')">×</span>` : ''}
                        </div>`;
                    });
                }

                feedHTML.innerHTML += `
                    <div class="post">
                        <div class="post-header">
                            <div class="post-author">${avatar} ${authorNick}</div>
                            <div class="post-time">${time}</div>
                        </div>
                        <div class="post-content">${contentText}</div>
                        ${post.image ? `<img src="${post.image}" class="post-image">` : ''}
                        
                        <div class="post-actions">
                            <button class="action-btn" style="${isLiked ? 'border-color:#ff4a5a; color:#ff4a5a;' : ''}" onclick="likePost('${post.id}', '${authorNick}')">❤️ <span>${likesCount}</span></button>
                            <button class="action-btn" onclick="toggleComments('${post.id}')">💬 Комменты</button>
                            ${authorNick === currentUser.nick ? `<button class="action-btn" onclick="db.ref('posts/${post.id}').remove()">🗑️ Стереть</button>` : ''}
                        </div>

                        <div class="comments-section" id="comments-${post.id}">
                            ${commentsHTML}
                            <div style="display:flex; gap:5px; margin-top:8px;">
                                <input type="text" id="commInput-${post.id}" placeholder="Текст ответа..." style="margin:0; font-size:13px; padding:8px;">
                                <button class="main-btn" style="width:60px; padding:8px; font-size:12px;" onclick="sendComment('${post.id}', '${authorNick}')">ОК</button>
                            </div>
                        </div>
                    </div>`;
            });
        }
    </script>
</body>
</html>
