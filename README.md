<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; line-height: 1.6; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Floating Nav Hub */
        .glass-nav { position: sticky; top: 15px; z-index: 2000; background: var(--glass); backdrop-filter: blur(20px); border-radius: 25px; padding: 15px; border: 1px solid var(--border); display: flex; justify-content: space-between; align-items: center; margin-bottom: 25px; }

        /* Multi-Page Card Style */
        .card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 35px; padding: 28px; margin-bottom: 25px; display: none; animation: fadeIn 0.5s ease; }
        .card.active { display: block; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        /* Hero & Stats */
        .profile-pfp { width: 120px; height: 120px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 25px rgba(0, 242, 254, 0.2); }
        .stat-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; margin-top: 20px; text-align: center; }
        .stat-val { color: var(--primary); font-size: 1.4rem; font-weight: 800; }
        .stat-lbl { font-size: 0.6rem; opacity: 0.5; text-transform: uppercase; }

        /* Language Toggle */
        .lang-btn { background: var(--primary); color: #000; padding: 5px 12px; border-radius: 50px; font-size: 0.7rem; font-weight: 800; cursor: pointer; }

        /* Unlimited Services */
        .service-pill { background: rgba(255,255,255,0.03); border: 1px solid var(--border); padding: 15px; border-radius: 20px; margin-bottom: 10px; display: flex; align-items: center; gap: 15px; }
        .service-pill i { font-size: 1.5rem; color: var(--primary); }

        /* Buttons */
        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; border-radius: 22px; font-weight: 800; width: 100%; border: none; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 10px; font-size: 1rem; }
        
        /* Footer Nav */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10,10,10,0.9); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 3000; }
        .nav-btn { color: white; opacity: 0.5; font-size: 1.3rem; cursor: pointer; }
        .nav-btn.active { color: var(--primary); opacity: 1; }
    </style>
</head>
<body>

    <div class="container">
        
        <nav class="glass-nav">
            <span style="font-weight: 800; font-size: 0.9rem; color: var(--primary);">PRIME SOLUTIONS</span>
            <div class="lang-btn" onclick="toggleLang()" id="langSwitcher">URDU MODE</div>
        </nav>

        <section id="home" class="card active">
            <div style="text-align: center;">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pfp">
                <h1 id="h-name" style="font-size: 2.2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
                <p id="h-tag" style="opacity: 0.7; font-weight: 300;">Digital Architect | CEO Prime Solutions</p>
                
                <div class="stat-grid">
                    <div class="stat-item"><div class="stat-val">150+</div><div id="s1" class="stat-lbl">Projects Done</div></div>
                    <div class="stat-item"><div class="stat-val">50+</div><div id="s2" class="stat-lbl">Global Clients</div></div>
                    <div class="stat-item"><div class="stat-val">5.0</div><div id="s3" class="stat-lbl">Rating ★</div></div>
                </div>
            </div>
            <button class="btn-main" style="margin-top: 25px;" onclick="showPage('contact')">
                <i class="fas fa-paper-plane"></i> <span id="h-btn">Get Started Now</span>
            </button>
        </section>

        <section id="services" class="card">
            <h3 id="serv-title"><i class="fas fa-layer-group"></i> Unlimited Services</h3>
            <p id="serv-desc" style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 20px;">International Standard Business Solutions</p>
            
            <div class="service-pill"><i class="fas fa-code"></i> <div><h4 id="v1">Full-Stack Development</h4><p style="font-size: 0.7rem; opacity: 0.6;">React, Firebase, & Modern Apps.</p></div></div>
            <div class="service-pill"><i class="fas fa-chart-line"></i> <div><h4 id="v2">Investment Portals</h4><p style="font-size: 0.7rem; opacity: 0.6;">Secure Finance & Profit Tracking.</p></div></div>
            <div class="service-pill"><i class="fas fa-shopping-cart"></i> <div><h4 id="v3">E-Commerce Hubs</h4><p style="font-size: 0.7rem; opacity: 0.6;">Multi-vendor & Secure Payments.</p></div></div>
            <div class="service-pill"><i class="fas fa-search-location"></i> <div><h4 id="v4">SEO & Ranking</h4><p style="font-size: 0.7rem; opacity: 0.6;">Global Google Ranking Mastery.</p></div></div>
        </section>

        <section id="contact" class="card">
            <h3 id="con-title">Let's Build Together</h3>
            <div style="margin-top: 20px;">
                <input type="text" id="cName" placeholder="Your Name" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); color: white; margin-bottom: 15px;">
                <textarea id="cMsg" rows="3" placeholder="Project Details" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); color: white; margin-bottom: 15px;"></textarea>
                <button class="btn-main" onclick="sendInquiry()" style="background: #25d366;">
                    <i class="fab fa-whatsapp"></i> <span id="con-btn">Send to WhatsApp</span>
                </button>
            </div>
        </section>

        <footer>
            <p>© 2026 PRIME SOLUTIONS | EXCELLENCE IN CODE</p>
            <p style="font-size: 0.6rem; opacity: 0.3; margin-top: 5px;">Trusted by 50+ Global Clients Worldwide</p>
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-btn active" onclick="showPage('home')"><i class="fas fa-home"></i></div>
        <div class="nav-btn" onclick="showPage('services')"><i class="fas fa-rocket"></i></div>
        <div class="nav-btn" onclick="showPage('contact')"><i class="fas fa-envelope"></i></div>
        <a href="tel:03705519562" class="nav-btn" style="text-decoration: none;"><i class="fas fa-phone-alt"></i></a>
    </nav>

    <script>
        let currentLang = 'en';

        function toggleLang() {
            const btn = document.getElementById('langSwitcher');
            if(currentLang === 'en') {
                btn.innerText = 'ENGLISH MODE';
                updateContent('ur');
                currentLang = 'ur';
            } else {
                btn.innerText = 'URDU MODE';
                updateContent('en');
                currentLang = 'en';
            }
        }

        function updateContent(lang) {
            const data = {
                en: {
                    name: "Muhammad Nazim", tag: "Digital Architect | CEO Prime Solutions",
                    s1: "Projects Done", s2: "Global Clients", s3: "Rating ★", btn1: "Get Started Now",
                    st: "Unlimited Services", sd: "International Standard Business Solutions",
                    v1: "Full-Stack Development", v2: "Investment Portals", v3: "E-Commerce Hubs", v4: "SEO & Ranking",
                    ct: "Let's Build Together", cb: "Send to WhatsApp"
                },
                ur: {
                    name: "محمد ناظم", tag: "ڈیجیٹل آرکیٹیکٹ | سی ای او پرائم سلوشنز",
                    s1: "مکمل پراجیکٹس", s2: "عالمی کلائنٹس", s3: "درجہ بندی ★", btn1: "ابھی شروع کریں",
                    st: "لامحدود سروسز", sd: "بین الاقوامی معیار کے بزنس سلوشنز",
                    v1: "ویب ڈویلپمنٹ", v2: "انویسٹمنٹ پورٹلز", v3: "ای کامرس اسٹورز", v4: "ایس ای او ماسٹری",
                    ct: "آئیے مل کر بنائیں", cb: "واٹس ایپ پر بھیجیں"
                }
            };
            const l = data[lang];
            document.getElementById('h-name').innerText = l.name;
            document.getElementById('h-tag').innerText = l.tag;
            document.getElementById('s1').innerText = l.s1;
            document.getElementById('s2').innerText = l.s2;
            document.getElementById('s3').innerText = l.s3;
            document.getElementById('h-btn').innerText = l.btn1;
            document.getElementById('serv-title').innerText = l.st;
            document.getElementById('serv-desc').innerText = l.sd;
            document.getElementById('v1').innerText = l.v1;
            document.getElementById('v2').innerText = l.v2;
            document.getElementById('v3').innerText = l.v3;
            document.getElementById('v4').innerText = l.v4;
            document.getElementById('con-title').innerText = l.ct;
            document.getElementById('con-btn').innerText = l.cb;
        }

        function showPage(id) {
            document.querySelectorAll('.card').forEach(c => c.classList.remove('active'));
            document.getElementById(id).classList.add('active');
            document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
            event.currentTarget.classList.add('active');
        }

        function sendInquiry() {
            const name = document.getElementById('cName').value;
            const msg = document.getElementById('cMsg').value;
            const text = `Hello Prime Solutions! I am ${name}. Project: ${msg}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
