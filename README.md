<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | CEO - Prime Solutions Global</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Vision Background */
        .vision-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; 
            background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 450px; height: 450px; background: var(--primary); filter: blur(200px); opacity: 0.12; border-radius: 50%; animation: pulse 12s infinite linear; }
        @keyframes pulse { from { transform: translate(-10%, -10%); } to { transform: translate(20%, 20%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 150px; }

        /* Sales Notification System (Working/Clickable) */
        #sales-notify { position: fixed; top: 15px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 90%; max-width: 420px; display: none; }
        .notify-pill { background: rgba(0, 0, 0, 0.96); border: 1px solid var(--primary); padding: 12px 18px; border-radius: 50px; backdrop-filter: blur(20px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 40px rgba(0,242,254,0.3); animation: slideIn 0.5s ease-out; cursor: pointer; }
        @keyframes slideIn { from { transform: translateY(-80px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        /* CEO Identity Card */
        .ceo-card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; text-align: center; position: relative; overflow: hidden; }
        .pfp-wrap { position: relative; width: 145px; height: 145px; margin: 0 auto 20px; }
        .pfp-img { width: 100%; height: 100%; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.35); transition: 0.4s; }
        .pfp-img:hover { transform: rotate(8deg) scale(1.05); }
        .online-led { position: absolute; bottom: 12px; right: 12px; width: 18px; height: 18px; background: #25d366; border-radius: 50%; border: 3px solid #000; box-shadow: 0 0 10px #25d366; animation: blink 1.5s infinite; }
        @keyframes blink { 0% { opacity: 1; } 50% { opacity: 0.4; } 100% { opacity: 1; } }

        /* Modern Tabs Navigation */
        .tab-menu { display: flex; justify-content: center; gap: 10px; margin: 30px 0; overflow-x: auto; padding-bottom: 10px; scrollbar-width: none; }
        .tab-btn { background: var(--glass); border: 1px solid var(--border); padding: 12px 25px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.85rem; transition: 0.3s; }
        .tab-btn.active { background: var(--primary); color: #000; border-color: var(--primary); font-weight: 800; }

        /* Content Views */
        .view-frame { display: none; }
        .view-frame.active { display: block; animation: zoomIn 0.4s cubic-bezier(0.18, 0.89, 0.32, 1.28); }
        @keyframes zoomIn { from { opacity: 0; transform: scale(0.96); } to { opacity: 1; transform: scale(1); } }

        /* Clickable Service Bricks */
        .service-brick { display: flex; align-items: center; gap: 20px; padding: 25px; background: rgba(255,255,255,0.02); border-radius: 30px; margin-bottom: 15px; text-decoration: none; color: white; border: 1px solid transparent; transition: 0.3s; }
        .service-brick:hover { border-color: var(--primary); background: rgba(0,242,254,0.08); transform: translateX(10px); }
        .service-brick i { font-size: 2.2rem; color: var(--primary); }
        .service-brick h4 { font-size: 1.1rem; margin-bottom: 4px; }
        .service-brick p { font-size: 0.75rem; opacity: 0.5; }

        /* Trust & Stats */
        .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; margin-top: 25px; }
        .stat-item { background: var(--glass); padding: 15px; border-radius: 22px; text-align: center; }
        .stat-item h2 { color: var(--primary); font-size: 1.6rem; }

        /* Social Hub Dock */
        .social-dock { display: flex; justify-content: center; gap: 12px; margin-top: 30px; }
        .social-link { width: 45px; height: 45px; background: var(--glass); border-radius: 15px; display: flex; align-items: center; justify-content: center; text-decoration: none; color: white; border: 1px solid var(--border); transition: 0.3s; }
        .social-link:hover { background: var(--primary); color: #000; transform: translateY(-5px); }

        /* Footer Navigation Dock */
        .nav-dock { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.95); backdrop-filter: blur(40px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,0.8); }
        .dock-icon { color: white; opacity: 0.35; font-size: 1.4rem; cursor: pointer; transition: 0.4s; }
        .dock-icon.active { opacity: 1; color: var(--primary); transform: translateY(-10px); text-shadow: 0 0 15px var(--primary); }

        /* Contact Engine */
        .input-group { background: rgba(0,0,0,0.3); border: 1px solid var(--border); border-radius: 25px; padding: 20px; margin-bottom: 12px; width: 100%; color: white; outline: none; transition: 0.3s; }
        .input-group:focus { border-color: var(--primary); box-shadow: 0 0 15px rgba(0,242,254,0.1); }
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 25px; width: 100%; border: none; font-weight: 800; font-size: 1rem; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 15px; text-decoration: none; }
    </style>
</head>
<body>

    <div class="vision-bg"><div class="glow"></div></div>

    <div id="sales-notify">
        <div class="notify-pill" onclick="navTo('contact')">
            <i class="fas fa-rocket"></i>
            <span id="notify-msg" style="font-size: 0.75rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        
        <section id="tab-home" class="view-frame active">
            <div class="ceo-card" data-aos="zoom-in">
                <div class="pfp-wrap">
                    <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-img" alt="Nazim">
                    <div class="online-led"></div>
                </div>
                <h1 style="font-size: 2.6rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px;">Muhammad Nazim</h1>
                <p style="opacity: 0.7; font-size: 0.85rem; margin-top: 5px;">Founder & Global CEO of Prime Solutions</p>
                
                <div class="social-dock">
                    <a href="https://facebook.com/prime.solutions" class="social-link"><i class="fab fa-facebook-f"></i></a>
                    <a href="https://instagram.com/nazim.prime" class="social-link"><i class="fab fa-instagram"></i></a>
                    <a href="https://linkedin.com/in/nazim-ceo" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                    <a href="https://github.com/web-hub-code" class="social-link"><i class="fab fa-github"></i></a>
                    <a href="https://wa.me/923332637235" class="social-link"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>

            <div class="stats-grid" data-aos="fade-up">
                <div class="stat-item"><h2>150+</h2><p style="font-size: 0.5rem; opacity: 0.5;">DONE</p></div>
                <div class="stat-item"><h2>50+</h2><p style="font-size: 0.5rem; opacity: 0.5;">GLOBAL</p></div>
                <div class="stat-item"><h2>5.0</h2><p style="font-size: 0.5rem; opacity: 0.5;">STARS</p></div>
            </div>
        </section>

        <section id="tab-products" class="view-frame">
            <h3 style="margin-bottom: 25px;"><i class="fas fa-boxes"></i> Industrial Software</h3>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-school"></i>
                <div><h4>School Management Pro</h4><p>Complete attendance, grading & fee system.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-dumbbell"></i>
                <div><h4>GYM Master 360</h4><p>Membership tracking & workout logs.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-hospital"></i>
                <div><h4>Hospital Ecosystem</h4><p>Patient records & billing automation.</p></div>
            </a>
        </section>

        <section id="tab-services" class="view-frame">
            <h3 style="margin-bottom: 25px;"><i class="fas fa-code"></i> Elite Development</h3>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-chart-pie"></i>
                <div><h4>Investment Portals</h4><p>Secure profit logs & ROI dashoards.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-mobile-screen"></i>
                <div><h4>Mobile-First Web Apps</h4><p>Fast, app-like experience on browser.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-brick">
                <i class="fas fa-search-dollar"></i>
                <div><h4>Global SEO Hub</h4><p>Ranking your business at #1 on Google.</p></div>
            </a>
        </section>

        <section id="tab-contact" class="view-frame">
            <div class="ceo-card" style="text-align: left; padding: 25px;">
                <h3>Start Your Project</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 20px;">Direct encrypted communication with Muhammad Nazim.</p>
                <input type="text" id="u-name" class="input-group" placeholder="Full Name / Brand">
                <textarea id="u-msg" rows="3" class="input-group" placeholder="Your Billion-Dollar Idea..."></textarea>
                
                <a href="javascript:void(0)" class="btn-action" onclick="launchWhatsApp()">
                    <i class="fab fa-whatsapp"></i> MESSAGE CEO NOW
                </a>
                <a href="tel:03705519562" class="btn-action" style="background: transparent; border: 1px solid var(--primary); color: var(--primary);">
                    <i class="fas fa-phone-alt"></i> CALL: 0370 5519562
                </a>
            </div>

            <div class="ceo-card" style="margin-top: 25px; text-align: left; padding: 20px;">
                <h4 style="margin-bottom: 10px;"><i class="fas fa-shield-alt"></i> Legal & Privacy</h4>
                <p style="font-size: 0.7rem; opacity: 0.6; line-height: 1.6;">
                    Prime Solutions ensures 100% data encryption. All projects are covered under a professional Non-Disclosure Agreement (NDA). We provide 24/7 dedicated support and a 100% success guarantee.
                </p>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.3; font-size: 0.65rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL HUB © 2026<br>
            Coded with Heart & Logic by Muhammad Nazim
        </footer>
    </div>

    <nav class="nav-dock">
        <div class="dock-icon active" onclick="navTo('home')"><i class="fas fa-home-alt"></i></div>
        <div class="dock-icon" onclick="navTo('products')"><i class="fas fa-briefcase"></i></div>
        <div class="dock-icon" onclick="navTo('services')"><i class="fas fa-cog"></i></div>
        <div class="dock-icon" onclick="navTo('contact')"><i class="fas fa-comments"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Sales Logic
        const users = ["Ali", "Sara", "John", "Fatima", "Chen", "Sofia", "Omar"];
        const cities = ["London", "Dubai", "New York", "Karachi", "Singapore"];
        const items = ["School System", "Investment Portal", "SEO Package", "GYM App"];

        function showSales() {
            const u = users[Math.floor(Math.random() * users.length)];
            const c = cities[Math.floor(Math.random() * cities.length)];
            const i = items[Math.floor(Math.random() * items.length)];
            
            document.getElementById('notify-msg').innerText = `${u} from ${c} just ordered a ${i}!`;
            const box = document.getElementById('sales-notify');
            box.style.display = 'block';
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(showSales, 10000);

        // Page Engine
        function navTo(page) {
            document.querySelectorAll('.view-frame').forEach(v => v.classList.remove('active'));
            document.getElementById('tab-' + page).classList.add('active');
            
            document.querySelectorAll('.dock-icon').forEach(i => i.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        // WhatsApp Strategy
        function launchWhatsApp() {
            const name = document.getElementById('u-name').value;
            const msg = document.getElementById('u-msg').value;
            const text = `Greetings CEO Nazim! I am ${name}. Project details: ${msg}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
