<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global Prime Solutions Official</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; line-height: 1.6; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Multi-Page Navigation Hub */
        .page-card { display: none; background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 28px; margin-bottom: 22px; animation: slideUp 0.6s ease; }
        .page-card.active { display: block; }
        @keyframes slideUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }

        /* Profile & Branding */
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 20px rgba(0, 242, 254, 0.3); }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        /* Stats & Trust Elements */
        .stats-grid { display: flex; justify-content: space-around; text-align: center; margin-top: 25px; }
        .stat-item h2 { color: var(--primary); font-size: 1.6rem; font-weight: 800; }
        .stat-item p { font-size: 0.6rem; opacity: 0.6; text-transform: uppercase; letter-spacing: 1px; }

        /* Language & UI Controls */
        .lang-toggle { position: fixed; top: 20px; right: 20px; z-index: 5000; background: var(--primary); color: #000; padding: 8px 15px; border-radius: 50px; font-weight: 800; font-size: 0.7rem; cursor: pointer; border: none; box-shadow: 0 5px 15px rgba(0, 242, 254, 0.3); }

        /* Process Steps */
        .step-box { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.03); padding: 15px; border-radius: 20px; border: 1px solid var(--border); }
        .step-id { background: var(--primary); color: #000; width: 32px; height: 32px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 800; font-size: 0.9rem; }

        /* Service Cards */
        .service-item { border-left: 3px solid var(--primary); padding-left: 15px; margin-bottom: 20px; }
        .service-item h4 { color: var(--primary); margin-bottom: 5px; }

        /* Contact & Buttons */
        .btn-action { background: linear-gradient(45deg, #25d366, #128c7e); color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 20px; border: none; font-size: 1rem; cursor: pointer; }

        /* Footer Bottom Bar */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 380px; background: rgba(10, 10, 10, 0.9); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 4000; box-shadow: 0 20px 40px rgba(0,0,0,0.5); }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.5; cursor: pointer; transition: 0.3s; }
        .nav-link.active { color: var(--primary); opacity: 1; transform: scale(1.2); }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <button class="lang-toggle" onclick="toggleLanguage()" id="langBtn">URDU MODE</button>

    <div class="container">
        
        <section id="home" class="page-card active">
            <div style="text-align: center;">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pic">
                <h1 class="gradient-text" id="userName">Muhammad Nazim</h1>
                <p id="userTag" style="opacity: 0.8; font-weight: 300;">Digital Architect | CEO Prime Solutions</p>
                
                <div class="stats-grid">
                    <div class="stat-item"><h2>150+</h2><p id="stat1">Projects Done</p></div>
                    <div class="stat-item"><h2>50+</h2><p id="stat2">Global Clients</p></div>
                    <div class="stat-item"><h2>5.0</h2><p id="stat3">Rating ★</p></div>
                </div>
            </div>
            <button class="btn-action" style="margin-top: 30px; background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000;" onclick="switchPage('services')">
                <i class="fas fa-arrow-right"></i> <span id="startBtn">Explore My Agency</span>
            </button>
        </section>

        <section id="services" class="page-card">
            <h3 id="servTitle"><i class="fas fa-rocket" style="color: var(--primary);"></i> Global Services</h3>
            <p id="servSub" style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 20px;">International Standard Business Solutions</p>
            
            <div class="service-item">
                <h4 id="s1t">Full-Stack Development</h4>
                <p id="s1d" style="font-size: 0.8rem; opacity: 0.7;">Modern websites using React, HTML, and high-security Firebase backends.</p>
            </div>
            <div class="service-item">
                <h4 id="s2t">Investment & Finance Portals</h4>
                <p id="s2d" style="font-size: 0.8rem; opacity: 0.7;">Professional investment systems with deposit/withdraw logs and profit tracking.</p>
            </div>
            <div class="service-item">
                <h4 id="s3t">Global SEO Mastery</h4>
                <p id="s3d" style="font-size: 0.8rem; opacity: 0.7;">Ranking your business on the first page of Google internationally.</p>
            </div>
            <div class="service-item">
                <h4 id="s4t">Branding & UI/UX</h4>
                <p id="s4d" style="font-size: 0.8rem; opacity: 0.7;">Creative designs that turn visitors into long-term loyal customers.</p>
            </div>
        </section>

        <section id="process" class="page-card">
            <h3 id="procTitle" style="margin-bottom: 20px;"><i class="fas fa-stream"></i> Working Process</h3>
            <div class="step-box"><div class="step-id">1</div><p id="p1" style="font-size: 0.8rem;"><b>Discovery:</b> Understanding your business goals perfectly.</p></div>
            <div class="step-box"><div class="step-id">2</div><p id="p2" style="font-size: 0.8rem;"><b>Design:</b> Creating unique UI/UX mobile-first prototypes.</p></div>
            <div class="step-box"><div class="step-id">3</div><p id="p3" style="font-size: 0.8rem;"><b>Develop:</b> Writing clean, fast, and SEO-optimized code.</p></div>
            <div class="step-box"><div class="step-id">4</div><p id="p4" style="font-size: 0.8rem;"><b>Launch:</b> Final testing and professional live deployment.</p></div>
        </section>

        <section id="contact" class="page-card">
            <h3 id="contTitle">Contact Prime Solutions</h3>
            <p id="contSub" style="font-size: 0.75rem; opacity: 0.6; margin-bottom: 20px;">Privacy & Trust Guaranteed | 24/7 Support</p>
            
            <div style="margin-top: 15px;">
                <input type="text" id="clientName" placeholder="Your Name" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); color: white; margin-bottom: 12px;">
                <textarea id="projectDesc" rows="3" placeholder="Tell us about your project" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); color: white; margin-bottom: 15px;"></textarea>
                
                <button class="btn-action" onclick="sendWhatsApp()">
                    <i class="fab fa-whatsapp"></i> <span id="waBtn">Send to WhatsApp</span>
                </button>
                <a href="tel:03705519562" class="btn-action" style="background: rgba(255,255,255,0.05); border: 1px solid var(--primary); color: var(--primary);">
                    <i class="fas fa-phone-alt"></i> Call: 0370 5519562
                </a>
            </div>
        </section>

        <footer id="footerText">
            © 2026 PRIME SOLUTIONS | EXCELLENCE IN EVERY CODE<br>
            Trusted by 50+ Global Clients Internationally
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-link active" onclick="switchPage('home')"><i class="fas fa-home"></i></div>
        <div class="nav-link" onclick="switchPage('services')"><i class="fas fa-rocket"></i></div>
        <div class="nav-link" onclick="switchPage('process')"><i class="fas fa-stream"></i></div>
        <div class="nav-link" onclick="switchPage('contact')"><i class="fas fa-paper-plane"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        let lang = 'en';

        function toggleLanguage() {
            const btn = document.getElementById('langBtn');
            if(lang === 'en') {
                updateUI('ur');
                btn.innerText = 'ENGLISH MODE';
                lang = 'ur';
            } else {
                updateUI('en');
                btn.innerText = 'URDU MODE';
                lang = 'en';
            }
        }

        function updateUI(l) {
            const translations = {
                en: {
                    name: "Muhammad Nazim", tag: "Digital Architect | CEO Prime Solutions",
                    s1: "Projects Done", s2: "Global Clients", s3: "Rating ★", start: "Explore My Agency",
                    servT: "Global Services", servS: "International Standard Business Solutions",
                    s1t: "Full-Stack Development", s1d: "Modern websites using React, HTML, and high-security Firebase backends.",
                    s2t: "Investment & Finance Portals", s2d: "Professional investment systems with deposit/withdraw logs and profit tracking.",
                    s3t: "Global SEO Mastery", s3d: "Ranking your business on the first page of Google internationally.",
                    s4t: "Branding & UI/UX", s4d: "Creative designs that turn visitors into long-term loyal customers.",
                    procT: "Working Process", p1: "Discovery: Understanding your business goals perfectly.",
                    p2: "Design: Creating unique UI/UX mobile-first prototypes.",
                    p3: "Develop: Writing clean, fast, and SEO-optimized code.",
                    p4: "Launch: Final testing and professional live deployment.",
                    contT: "Contact Prime Solutions", contS: "Privacy & Trust Guaranteed | 24/7 Support",
                    wa: "Send to WhatsApp", foot: "© 2026 PRIME SOLUTIONS | EXCELLENCE IN EVERY CODE"
                },
                ur: {
                    name: "محمد ناظم", tag: "ڈیجیٹل آرکیٹیکٹ | سی ای او پرائم سلوشنز",
                    s1: "مکمل پراجیکٹس", s2: "عالمی کلائنٹس", s3: "درجہ بندی ★", start: "ایجنسی کا دورہ کریں",
                    servT: "عالمی سروسز", servS: "بین الاقوامی معیار کے بزنس سلوشنز",
                    s1t: "فل اسٹیک ڈویلپمنٹ", s1d: "React اور Firebase کے ساتھ جدید اور محفوظ ویب سائٹس۔",
                    s2t: "انویسٹمنٹ پورٹلز", s2d: "منافع اور ڈیپازٹ ٹریکنگ کے ساتھ پروفیشنل انویسٹمنٹ سسٹمز۔",
                    s3t: "عالمی ایس ای او", s3d: "گوگل کے پہلے پیج پر آپ کے بزنس کی عالمی رینکنگ۔",
                    s4t: "برانڈنگ اور ڈیزائن", s4d: "ایسے ڈیزائن جو کلائنٹس کو آپ کا دیوانہ بنا دیں۔",
                    procT: "کام کرنے کا طریقہ", p1: "تحقیق: آپ کے بزنس کے مقاصد کو مکمل سمجھنا۔",
                    p2: "ڈیزائن: موبائل کے لیے بہترین اور منفرد ڈیزائن بنانا۔",
                    p3: "کوڈنگ: تیز رفتار اور سرچ انجن کے لیے بہترین کوڈنگ۔",
                    p4: "لانچ: فائنل ٹیسٹنگ اور ویب سائٹ لائیو کرنا۔",
                    contT: "رابطہ کریں", contS: "پرائیویسی اور اعتماد کی مکمل ضمانت",
                    wa: "واٹس ایپ پر بھیجیں", foot: "© 2026 پرائم سلوشنز | ہر کوڈ میں مہارت"
                }
            };
            const t = translations[l];
            document.getElementById('userName').innerText = t.name;
            document.getElementById('userTag').innerText = t.tag;
            document.getElementById('stat1').innerText = t.s1;
            document.getElementById('stat2').innerText = t.s2;
            document.getElementById('stat3').innerText = t.s3;
            document.getElementById('startBtn').innerText = t.start;
            document.getElementById('servTitle').innerText = t.servT;
            document.getElementById('servSub').innerText = t.servS;
            document.getElementById('s1t').innerText = t.s1t; document.getElementById('s1d').innerText = t.s1d;
            document.getElementById('s2t').innerText = t.s2t; document.getElementById('s2d').innerText = t.s2d;
            document.getElementById('s3t').innerText = t.s3t; document.getElementById('s3d').innerText = t.s3d;
            document.getElementById('s4t').innerText = t.s4t; document.getElementById('s4d').innerText = t.s4d;
            document.getElementById('procTitle').innerText = t.procT;
            document.getElementById('p1').innerHTML = t.p1; document.getElementById('p2').innerHTML = t.p2;
            document.getElementById('p3').innerHTML = t.p3; document.getElementById('p4').innerHTML = t.p4;
            document.getElementById('contTitle').innerText = t.contT;
            document.getElementById('contSub').innerText = t.contS;
            document.getElementById('waBtn').innerText = t.wa;
            document.getElementById('footerText').innerHTML = t.foot + "<br>Trusted by 50+ Global Clients Internationally";
        }

        function switchPage(pageId) {
            document.querySelectorAll('.page-card').forEach(p => p.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
            document.querySelectorAll('.nav-link').forEach(l => l.classList.remove('active'));
            const navIcons = { home:0, services:1, process:2, contact:3 };
            document.querySelectorAll('.nav-link')[navIcons[pageId]].classList.add('active');
            window.scrollTo(0,0);
        }

        function sendWhatsApp() {
            const name = document.getElementById('clientName').value;
            const desc = document.getElementById('projectDesc').value;
            const text = `Hello Nazim! My name is ${name}. Project Inquiry: ${desc}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
