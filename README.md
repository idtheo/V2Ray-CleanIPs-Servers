<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>V2Ray Clean IPs & Servers - لیست IP تمیز و کانفیگ</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Segoe UI', Tahoma, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
        }
        .container { max-width: 1200px; margin: 0 auto; }
        header {
            text-align: center;
            color: white;
            margin-bottom: 40px;
            animation: fadeInDown 1s ease;
        }
        .lang-toggle {
            background: rgba(255,255,255,0.2);
            border: none;
            color: white;
            padding: 12px 24px;
            border-radius: 50px;
            font-size: 16px;
            cursor: pointer;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }
        .lang-toggle:hover { transform: scale(1.05); background: rgba(255,255,255,0.3); }
        .content {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
            animation: fadeInUp 1s ease 0.3s both;
        }
        h1 { font-size: 2.5em; margin-bottom: 10px; color: #333; }
        h2 { color: #667eea; margin: 30px 0 15px; }
        ul { list-style: none; padding: 0; }
        li {
            background: #f8f9ff;
            margin: 10px 0;
            padding: 15px;
            border-radius: 12px;
            border-left: 5px solid #667eea;
            transition: all 0.3s ease;
        }
        li:hover { transform: translateX(-5px); box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
        .emoji { font-size: 1.5em; margin-left: 10px; }
        .fadeInUp { animation: fadeInUp 0.8s ease; }
        @keyframes fadeInDown { from { opacity: 0; transform: translateY(-30px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
        @media (max-width: 768px) { .content { padding: 20px; } h1 { font-size: 2em; } }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1 id="title">لیست روزانه IP های تمیز و کانفیگ‌های V2Ray/Xray</h1>
            <button class="lang-toggle" onclick="toggleLang()">🇺🇸 English</button>
        </header>
        
        <div class="content">
            <h2>🚀 ویژگی‌های شگفت‌انگیز:</h2>
            <ul>
                <li>📡 <strong>IP های کاملاً تمیز</strong> - بدون بلاک و فیلتر<span class="emoji">✅</span></li>
                <li>⚡ <strong>سرعت بالا و پایداری عالی</strong> - تست‌شده در ایران<span class="emoji">🏆</span></li>
                <li>🔄 <strong>آپدیت خودکار هر ۲۴ ساعت</strong> - همیشه تازه<span class="emoji">🆕</span></li>
                <li>📱 <strong>سازگار با v2rayNG, Hiddify, FoXray</strong><span class="emoji">🎮</span></li>
                <li>🌍 <strong>بهینه‌شده برای دور زدن فیلترینگ</strong> - کار می‌کنه! <span class="emoji">🔥</span></li>
                <li>💎 <strong>رایگان و عمومی</strong> (تا وقتی لازم باشه 🥱)<span class="emoji">🎁</span></li>
            </ul>

            <h2>📋 نحوه استفاده:</h2>
            <ul>
                <li>📥 کانفیگ‌ها رو کپی کن</li>
                <li>➕ در v2rayNG یا Hiddify Import کن</li>
                <li>▶️ Connect بزن و لذت ببر! 🚀</li>
            </ul>

            <h2>⭐ چرا ما؟</h2>
            <p>بهترین لیست تمیزترین IPها و سریع‌ترین سرورها رو هر روز برات جمع می‌کنیم. <strong>ستاره بده و Watch کن</strong> تا همیشه آپدیت باشی! 🌟</p>
            
            <div style="text-align: center; margin-top: 30px;">
                <p><strong>آخرین آپدیت:</strong> <span id="lastUpdate">26 ژانویه 2026</span></p>
            </div>
        </div>
    </div>

    <script>
        const persian = {
            title: "لیست روزانه IP های تمیز و کانفیگ‌های V2Ray/Xray",
            features: "🚀 ویژگی‌های شگفت‌انگیز:",
            feat1: "📡 <strong>IP های کاملاً تمیز</strong> - بدون بلاک و فیلتر",
            feat2: "⚡ <strong>سرعت بالا و پایداری عالی</strong> - تست‌شده در ایران",
            feat3: "🔄 <strong>آپدیت خودکار هر ۲۴ ساعت</strong> - همیشه تازه",
            feat4: "📱 <strong>سازگار با v2rayNG, Hiddify, FoXray</strong>",
            feat5: "🌍 <strong>بهینه‌شده برای دور زدن فیلترینگ</strong> - کار می‌کنه!",
            feat6: "💎 <strong>رایگان و عمومی</strong> (تا وقتی لازم باشه 🥱)",
            howto: "📋 نحوه استفاده:",
            step1: "📥 کانفیگ‌ها رو کپی کن",
            step2: "➕ در v2rayNG یا Hiddify Import کن",
            step3: "▶️ Connect بزن و لذت ببر! 🚀",
            why: "⭐ چرا ما؟",
            desc: "بهترین لیست تمیزترین IPها و سریع‌ترین سرورها رو هر روز برات جمع می‌کنیم. <strong>ستاره بده و Watch کن</strong> تا همیشه آپدیت باشی! 🌟",
            lastUpdate: "آخرین آپدیت:",
            date: "26 ژانویه 2026",
            btn: "🇺🇸 English"
        };

        const english = {
            title: "Daily Clean IPs & V2Ray/Xray Server Configs List",
            features: "🚀 Amazing Features:",
            feat1: "📡 <strong>Fully Clean IPs</strong> - No blocks or filters",
            feat2: "⚡ <strong>High Speed & Great Stability</strong> - Tested in Iran",
            feat3: "🔄 <strong>Auto-updated every 24h</strong> - Always fresh",
            feat4: "📱 <strong>Compatible with v2rayNG, Hiddify, FoXray</strong>",
            feat5: "🌍 <strong>Optimized for censorship bypass</strong> - It works!",
            feat6: "💎 <strong>Free & Public</strong> (as long as needed 🥱)",
            howto: "📋 How to Use:",
            step1: "📥 Copy the configs",
            step2: "➕ Import to v2rayNG or Hiddify",
            step3: "▶️ Hit Connect & Enjoy! 🚀",
            why: "⭐ Why Us?",
            desc: "We collect the cleanest IPs & fastest servers daily for you. <strong>Star & Watch</strong> to stay updated! 🌟",
            lastUpdate: "Last Update:",
            date: "January 26, 2026",
            btn: "🇮🇷 فارسی"
        };

        let isEnglish = false;
        function toggleLang() {
            isEnglish = !isEnglish;
            const lang = isEnglish ? english : persian;
            document.getElementById('title').innerHTML = lang.title;
            document.querySelector('h2:nth-of-type(1)').innerHTML = lang.features;
            document.querySelectorAll('li')[0].innerHTML = lang.feat1 + '<span class="emoji">✅</span>';
            document.querySelectorAll('li')[1].innerHTML = lang.feat2 + '<span class="emoji">🏆</span>';
            document.querySelectorAll('li')[2].innerHTML = lang.feat3 + '<span class="emoji">🆕</span>';
            document.querySelectorAll('li')[3].innerHTML = lang.feat4 + '<span class="emoji">🎮</span>';
            document.querySelectorAll('li')[4].innerHTML = lang.feat5 + '<span class="emoji">🔥</span>';
            document.querySelectorAll('li')[5].innerHTML = lang.feat6 + '<span class="emoji">🎁</span>';
            document.querySelector('h2:nth-of-type(2)').innerHTML = lang.howto;
            document.querySelectorAll('li')[6].innerHTML = lang.step1;
            document.querySelectorAll('li')[7].innerHTML = lang.step2;
            document.querySelectorAll('li')[8].innerHTML = lang.step3;
            document.querySelector('h2:nth-of-type(3)').innerHTML = lang.why;
            document.querySelector('p').innerHTML = lang.desc;
            document.querySelector('strong').innerHTML = lang.lastUpdate;
            document.getElementById('lastUpdate').textContent = lang.date;
            document.querySelector('.lang-toggle').textContent = lang.btn;
            
            // RTL/LTR switch
            document.body.dir = isEnglish ? 'ltr' : 'rtl';
            document.documentElement.lang = isEnglish ? 'en' : 'fa';
        }
    </script>
</body>
</html>
