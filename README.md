<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global CEO - Prime Solutions Hub</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Vision Background */
        .vision-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001a1d 0%, #010204 100%); }
        .glow-orb { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: drift 20s infinite linear; }
        @keyframes drift { from { transform: rotate(0deg) translateX(100px) rotate(0deg); } to { transform: rotate(360deg) translateX(100px) rotate(-360deg); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 130px; }

        /* Advanced Multi-Page Engine */
        .page-hub { display: none; animation: reveal 0.7s cubic-bezier(0.19, 1, 0.22, 1) forwards; }
        .page-hub.active { display: block; }
        @keyframes reveal { from { opacity: 0; transform: translateY(40px) scale(0.98); } to { opacity: 1; transform: translateY(0) scale(1); } }

        /* CEO Premium Branding */
        .ceo-card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; text-align: center; position: relative; overflow: hidden; box-shadow: 0 25px 50px rgba(0,0,0,0.4); }
        .ceo-card::after { content: ''; position: absolute; top: -10%; right: -10%; width: 100px; height: 100px; background: var(--primary); filter: blur(60px); opacity: 0.3; }
        
        .pfp-main { width: 145px; height: 145px; border-radius: 50%; border: 4px solid var(--primary); padding: 6px; box-shadow: 0 0 45px rgba(0, 242, 254, 0.25); margin-bottom: 25px; transition: 0.5s; }
        .pfp-main:hover { transform: rotate(5deg) scale(1.05); }

        .master-name { font-size: 2.7rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        /* Global Market Stats */
        .market-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; margin-top: 35px; }
        .m-item { background: rgba(255,255,255,0.02); padding: 15px 5px; border-radius: 25px; border: 1px solid var(--border); }
        .m-item h4 { font-size: 1.7rem; color: var(--primary); margin-bottom: 2px; }
        .m-item p { font-size: 0.5rem; opacity: 0.5; text-transform: uppercase; letter-spacing: 1.5px; }

        /* Infinity Services Grid */
        .service-tile { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-top: 25px; transition: 0.4s; }
        .row-item { display: flex; align-items: center; gap: 20px; margin-bottom: 22px; padding: 20px; background: rgba(255,255,255,0.02); border-radius: 25px; border: 1px solid transparent; transition: 0.3s; }
        .row-item:hover { border-color: var(--primary); background: rgba(0, 242, 254, 0.08); transform: translateX(10px); }
        .row-item i { font-size: 2rem; color: var(--primary); text-shadow: 0 0 15px var(--primary); }

        /* Future Dock Navigation */
        .nav-dock { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.9); backdrop-filter: blur(35px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 20px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,0.8); }
        .dock-link { color: white; opacity: 0.3; font-size: 1.5rem; cursor: pointer; transition: 0.4s; position: relative; }
        .dock-link.active { opacity: 1; color: var(--primary); transform: translateY(-8px); }
        .dock-link.active::before { content: ''; position: absolute; bottom: -12px; left: 50%; transform: translateX(-50%); width: 25px; height: 4px; background: var(--primary); border-radius: 10px; box-shadow: 0 0 15px var(--primary); }

        /* High-Conversion Buttons */
        .btn-mega { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 28px; width: 100%; border: none; font-weight: 800; font-size: 1.1rem; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 15px; margin-top: 30px; transition: 0.3s; }
        .btn-mega:active { transform: scale(0.95); }

        /* AI Status Floating */
        .status-pill { position: fixed; top: 25px; left: 50%; transform: translateX(-50%); background: var(--glass); backdrop-filter: blur(15px); border: 1px solid var(--border); padding: 8px 20px; border-radius: 50px; font-size: 0.65rem; font-weight: 800; z-index: 1000; letter-spacing: 1px; display: flex; align-items: center; gap: 8px; }
        .dot { height: 8px; width: 8px; background: #25d366; border-radius: 50%; box-shadow: 0 0 12px #25d366; animation: pulse 1.5s infinite; }
    </style>
</head>
<body>

    <div class="vision-bg"><div class="glow-orb"></div></div>

    <div class="status-pill">
        <span class="dot"></span> GLOBAL CEO ONLINE
    </div>

    <div class="container">
        
        <div style="display: flex; justify-content: flex-end; margin-bottom: 20px;">
            <button onclick="toggleMasterLang()" id="langSwitcher" style="background: var(--primary); color: #000; border: none; padding: 6px 18px; border-radius: 50px; font-weight: 800; font-size: 0.7rem; cursor: pointer;">SWITCH TO URDU</button>
        </div>

        <section id="view-home" class="page-hub active">
            <div class="ceo-card" data-aos="zoom-in">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="pfp-main">
                <h1 class="master-name" id="l-name">Muhammad Nazim</h1>
                <p id="l-tag" style="opacity: 0.7; font-weight: 300; margin-top: 5px;">Architect of Digital Empires | CEO Prime Solutions</p>
                
                <div class="market-grid">
                    <div class="m-item"><h4>150+</h4><p id="s1">Completed</p></div>
                    <div class="m-item"><h4>50+</h4><p id="s2">Global Clients</p></div>
                    <div class="m-item"><h4>5.0</h4><p id="s3">Success Rate</p></div>
                </div>
            </div>

            <div class="service-tile" data-aos="fade-up">
                <h3 id="l-mission"><i class="fas fa-bolt"></i> Our Vision 2026</h3>
                <p id="l-desc" style="font-size: 0.85rem; opacity: 0.6; margin-top: 15px; line-height: 1.8;">Prime Solutions ka maqsad dunya ki #1 agency banna hai. Hum sirf website nahi banate, hum aapke business ko aik international brand mein convert karte hain.</p>
                <button class="btn-mega" onclick="navTo('contact')">
                    <span id="l-btn1">START YOUR EMPIRE</span> <i class="fas fa-chevron-right"></i>
                </button>
            </div>
        </section>

        <section id="view-services" class="page-hub">
            <h3 style="margin-bottom: 25px; padding-left: 10px;" id="l-stit"><i class="fas fa-atom"></i> Specialized Units</h3>
            <div class="row-item">
                <i class="fas fa-layer-group"></i>
                <div><h4 id="v1">Next-Gen Full Stack</h4><p style="font-size: 0.75rem; opacity: 0.6;">High-speed React & Node.js ecosystems.</p></div>
            </div>
            <div class="row-item">
                <i class="fas fa-shield-halved"></i>
                <div><h4 id="v2">FinTech & Security</h4><p style="font-size: 0.75rem; opacity: 0.6;">Secure investment platforms with AI logs.</p></div>
            </div>
            <div class="row-item">
                <i class="fas fa-chart-pie"></i>
                <div><h4 id="v3">International SEO</h4><p style="font-size: 0.75rem; opacity: 0.6;">Global ranking strategies for top traffic.</p></div>
            </div>
        </section>

        <section id="view-contact" class="page-hub">
            <div class="ceo-card">
                <h3 id="l-ctitle">Global Inquiry Hub</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 25px;" id="l-csub">Direct encrypted communication with the CEO.</p>
                
                <input type="text" id="iName" placeholder="Full Name / Brand" style="width: 100%; padding: 22px; border-radius: 22px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none; transition: 0.3s;" onfocus="this.style.borderColor='var(--primary)'">
                <textarea id="iDesc" rows="3" placeholder="Describe your billion-dollar idea..." style="width: 100%; padding: 22px; border-radius: 22px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 20px; outline: none; transition: 0.3s;" onfocus="this.style.borderColor='var(--primary)'"></textarea>
                
                <button class="btn-mega" onclick="launchStrategy()">
                    <i class="fab fa-whatsapp"></i> <span id="l-cbtn">BOOK STRATEGY CALL</span>
                </button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 60px; opacity: 0.2; font-size: 0.65rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL CONGLOMERATE © 2026<br>
            Coded with Heart & Logic by Muhammad Nazim
        </footer>
    </div>

    <nav class="nav-dock">
        <div class="dock-link active" onclick="navTo('home')"><i class="fas fa-home-lg-alt"></i></div>
        <div class="dock-link" onclick="navTo('services')"><i class="fas fa-grid-2"></i></div>
        <div class="dock-link" onclick="navTo('contact')"><i class="fas fa-paper-plane"></i></div>
        <a href="tel:03705519562" class="dock-link" style="text-decoration:none;"><i class="fas fa-phone-office"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1200, once: true });
        let currentLang = 'en';

        function navTo(page) {
            document.querySelectorAll('.page-hub').forEach(p => p.classList.remove('active'));
            document.getElementById('view-' + page).classList.add('active');
            document.querySelectorAll('.dock-link').forEach(l => l.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        function toggleMasterLang() {
            const btn = document.getElementById('langSwitcher');
            if(currentLang === 'en') {
                applyLang('ur');
                btn.innerText = 'SWITCH TO ENGLISH';
                currentLang = 'ur';
            } else {
                applyLang('en');
                btn.innerText = 'SWITCH TO URDU';
                currentLang = 'en';
            }
        }

        function applyLang(l) {
            const dictionary = {
                en: { name:"Muhammad Nazim", tag:"Architect of Digital Empires | CEO Prime Solutions", s1:"Completed", s2:"Global Clients", s3:"Success Rate", miss:"Our Vision 2026", desc:"Prime Solutions ka maqsad dunya ki #1 agency banna hai. Hum sirf website nahi banate, hum aapke business ko aik international brand mein convert karte hain.", btn1:"START YOUR EMPIRE", stit:"Specialized Units", v1:"Next-Gen Full Stack", v2:"FinTech & Security", v3:"International SEO", ct:"Global Inquiry Hub", cs:"Direct encrypted communication with the CEO.", cb:"BOOK STRATEGY CALL" },
                ur: { name:"محمد ناظم", tag:"ڈیجیٹل سلطنتوں کے معمار | سی ای او پرائم سلوشنز", s1:"مکمل پراجیکٹس", s2:"عالمی کلائنٹس", s3:"کامیابی کی شرح", miss:"ہمارا وژن 2026", desc:"پرائم سلوشنز کا مقصد دنیا کی #1 ایجنسی بننا ہے۔ ہم صرف ویب سائٹ نہیں بناتے، ہم آپ کے بزنس کو ایک بین الاقوامی برانڈ میں تبدیل کرتے ہیں۔", btn1:"اپنی سلطنت شروع کریں", stit:"خصوصی یونٹس", v1:"جدید فل اسٹیک ڈویلپمنٹ", v2:"فنانشل اور سیکیورٹی پورٹلز", v3:"عالمی ایس ای او رینکنگ", ct:"عالمی انکوائری مرکز", cs:"سی ای او کے ساتھ براہ راست اور محفوظ رابطہ۔", cb:"سٹریٹیجی کال بک کریں" }
            };
            const d = dictionary[l];
            document.getElementById('l-name').innerText = d.name;
            document.getElementById('l-tag').innerText = d.tag;
            document.getElementById('s1').innerText = d.s1;
            document.getElementById('s2').innerText = d.s2;
            document.getElementById('s3').innerText = d.s3;
            document.getElementById('l-mission').innerHTML = `<i class="fas fa-bolt"></i> ${d.miss}`;
            document.getElementById('l-desc').innerText = d.desc;
            document.getElementById('l-btn1').innerText = d.btn1;
            document.getElementById('l-stit').innerHTML = `<i class="fas fa-atom"></i> ${d.stit}`;
            document.getElementById('v1').innerText = d.v1;
            document.getElementById('v2').innerText = d.v2;
            document.getElementById('v3').innerText = d.v3;
            document.getElementById('l-ctitle').innerText = d.ct;
            document.getElementById('l-csub').innerText = d.cs;
            document.getElementById('l-cbtn').innerText = d.cb;
        }

        function launchStrategy() {
            const name = document.getElementById('iName').value;
            const desc = document.getElementById('iDesc').value;
            const text = `Greetings CEO Nazim! My name is ${name}. I am interested in building a world-class project: ${desc}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
