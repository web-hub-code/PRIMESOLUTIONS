<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Infinity</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #fdfdfd; --text: #1d1d1f; --card: rgba(255, 255, 255, 0.85); --border: rgba(0, 0, 0, 0.08);
            --glow: rgba(79, 172, 254, 0.3);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
            --glow: rgba(79, 172, 254, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: background 0.4s ease, color 0.4s ease; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; scroll-behavior: smooth; }

        /* Progress Bar & Background Mesh */
        #scroll-progress { position: fixed; top: 0; left: 0; width: 0%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); z-index: 9999; border-radius: 0 5px 5px 0; }
        .bg-mesh { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background-image: radial-gradient(var(--primary) 0.5px, transparent 0.5px); background-size: 30px 30px; opacity: 0.05; }

        /* Floating Controls */
        .theme-toggle { position: fixed; top: 20px; right: 20px; z-index: 2000; background: var(--card); border: 1px solid var(--border); padding: 12px; border-radius: 50%; cursor: pointer; backdrop-filter: blur(15px); color: var(--primary); box-shadow: 0 8px 20px rgba(0,0,0,0.1); }
        .ai-support { position: fixed; bottom: 100px; right: 20px; z-index: 2000; background: var(--primary); color: white; width: 55px; height: 55px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.5rem; box-shadow: 0 10px 25px var(--glow); cursor: pointer; animation: pulse 2s infinite; }

        @keyframes pulse { 0% { transform: scale(1); box-shadow: 0 0 0 0 var(--glow); } 70% { transform: scale(1.1); box-shadow: 0 0 0 15px rgba(0,0,0,0); } 100% { transform: scale(1); } }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 50px 15px 120px; }

        /* Infinity Card System */
        .card { 
            background: var(--card); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 28px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 30px rgba(0,0,0,0.03); position: relative;
        }
        .card:hover { transform: translateY(-12px); border-color: var(--primary); box-shadow: 0 20px 45px var(--glow); }

        /* Trust Badge Hero */
        .verify-tag { background: rgba(37, 211, 102, 0.1); color: #25d366; padding: 6px 15px; border-radius: 50px; font-size: 0.65rem; font-weight: 800; display: inline-block; margin-bottom: 15px; border: 1px solid rgba(37, 211, 102, 0.2); }
        .profile-img { width: 130px; height: 130px; border-radius: 50%; border: 4px solid #fff; box-shadow: 0 15px 30px rgba(0,0,0,0.1); margin-bottom: 15px; }
        .glitch-text { background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.4rem; letter-spacing: -1px; }

        /* Unlimited Features Grid */
        .feature-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 20px; }
        .f-item { background: rgba(0,0,0,0.02); padding: 15px; border-radius: 20px; border: 1px solid var(--border); text-align: center; cursor: pointer; }
        .f-item i { font-size: 1.5rem; color: var(--primary); margin-bottom: 8px; }
        .f-item p { font-size: 0.75rem; font-weight: 600; }
        .f-item:hover { background: var(--primary); color: white; }
        .f-item:hover i { color: white; }

        /* Conversion Pricing */
        .pricing-box { background: linear-gradient(135deg, var(--primary), var(--secondary)); color: white; border-radius: 30px; padding: 25px; margin-top: 15px; text-align: center; }
        .price-list { text-align: left; font-size: 0.8rem; margin: 15px 0; list-style: none; opacity: 0.9; }
        .price-list li { margin-bottom: 8px; }

        /* Interactive Action Buttons */
        .action-btn { display: flex; align-items: center; justify-content: center; gap: 12px; padding: 20px; border-radius: 25px; font-weight: 800; text-decoration: none; margin-top: 15px; font-size: 1rem; border: none; cursor: pointer; transition: 0.3s; }
        .wa-btn { background: #25d366; color: white; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); }
        .call-btn { background: var(--text); color: var(--bg); }
        .action-btn:hover { transform: scale(1.03); filter: brightness(1.1); }

        /* Bottom Menu */
        .bottom-menu { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 88%; max-width: 400px; background: var(--card); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .menu-link { color: var(--text); opacity: 0.5; font-size: 1.4rem; transition: 0.3s; text-decoration: none; }
        .menu-link:hover, .menu-link.active { color: var(--primary); opacity: 1; transform: translateY(-3px); }
    </style>
</head>
<body data-theme="light">

    <div id="scroll-progress"></div>
    <div class="bg-mesh"></div>

    <div class="theme-toggle" onclick="toggleTheme()" title="Switch Theme"><i class="fas fa-moon"></i></div>
    <div class="ai-support" onclick="location.href='https://wa.me/923332637235'"><i class="fas fa-robot"></i></div>

    <div class="container">
        
        <section class="card hero" style="text-align: center;" data-aos="zoom-in">
            <div class="verify-tag"><i class="fas fa-shield-check"></i> VERIFIED PLATFORM & OWNER</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-img">
            <h1 class="glitch-text">Muhammad Nazim</h1>
            <p style="opacity: 0.7; font-weight: 400; font-size: 1rem;">Founder | Prime Solutions Official</p>
            
            <div style="display: flex; justify-content: center; gap: 15px; margin-top: 20px;">
                <div style="text-align: center;"><h2 style="color: var(--primary);">50+</h2><p style="font-size: 0.6rem; opacity: 0.5;">PROJECTS</p></div>
                <div style="height: 30px; width: 1px; background: var(--border);"></div>
                <div style="text-align: center;"><h2 style="color: var(--primary);">100%</h2><p style="font-size: 0.6rem; opacity: 0.5;">SATISFACTION</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-star" style="color: #ffca28;"></i> Mastery & Expertise</h3>
            <div class="feature-grid">
                <div class="f-item"><i class="fas fa-laptop-code"></i><p>Full-Stack</p></div>
                <div class="f-item"><i class="fas fa-mobile-alt"></i><p>App Design</p></div>
                <div class="f-item"><i class="fas fa-search-dollar"></i><p>SEO Expert</p></div>
                <div class="f-item"><i class="fas fa-database"></i><p>Firebase</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-rocket"></i> Agency Packages</h3>
            <div class="pricing-box">
                <span style="font-size: 0.7rem; letter-spacing: 2px;">STARTING JOURNEY AT</span>
                <h2 style="font-size: 2.5rem;">$49 <small style="font-size: 0.9rem; font-weight: 300;">/project</small></h2>
                <ul class="price-list">
                    <li><i class="fas fa-check-circle"></i> Free Domain & Hosting Setup</li>
                    <li><i class="fas fa-check-circle"></i> Mobile-First UI Responsive</li>
                    <li><i class="fas fa-check-circle"></i> Lifetime Bug Support</li>
                </ul>
                <button onclick="location.href='https://wa.me/923332637235'" style="background: white; color: var(--primary); border: none; padding: 12px 30px; border-radius: 50px; font-weight: 800; cursor: pointer;">BOOK NOW</button>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-user-check"></i> Client Success</h3>
            <div style="background: rgba(0,0,0,0.02); padding: 15px; border-radius: 20px; border-left: 5px solid var(--primary); margin-top: 15px;">
                <p style="font-size: 0.8rem; font-style: italic; opacity: 0.8;">"Prime Solutions ne mera business portal (Pakgold) sirf 48 hours mein live kar diya. Amazing quality!"</p>
                <p style="font-size: 0.6rem; text-align: right; margin-top: 5px; font-weight: 800; color: var(--primary);">— Verified Client</p>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 6px solid var(--primary);">
            <h3 style="text-align: center;">Let's Build Greatness</h3>
            <p style="text-align: center; font-size: 0.8rem; opacity: 0.6; margin: 10px 0 20px;">Available 24/7 for International Clients</p>
            
            <a href="https://wa.me/923332637235" class="action-btn wa-btn">
                <i class="fab fa-whatsapp"></i> Direct WhatsApp
            </a>
            
            <a href="tel:03705519562" class="action-btn call-btn">
                <i class="fas fa-phone-alt"></i> Call Now: 0370 5519562
            </a>

            <div style="text-align: center; margin-top: 25px; display: flex; justify-content: center; gap: 20px;">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" style="color: #1877F2; font-size: 1.5rem;"><i class="fab fa-facebook"></i></a>
                <a href="mailto:webhub262@gmail.com" style="color: #ea4335; font-size: 1.5rem;"><i class="fas fa-envelope"></i></a>
                <a href="https://github.com/PrimeSolutionsOfficial" style="color: var(--text); font-size: 1.5rem;"><i class="fab fa-github"></i></a>
            </div>
        </div>

        <footer style="text-align: center; font-size: 0.75rem; opacity: 0.4; line-height: 1.8;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Coded with Precision by Muhammad Nazim
        </footer>
    </div>

    <nav class="bottom-menu">
        <a href="#" class="menu-link active"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="menu-link"><i class="fab fa-whatsapp"></i></a>
        <a href="tel:03705519562" class="menu-link"><i class="fas fa-phone-volume"></i></a>
        <a href="mailto:webhub262@gmail.com" class="menu-link"><i class="fas fa-envelope-open-text"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Theme Toggle Logic
        function toggleTheme() {
            const body = document.body;
            const icon = document.querySelector('.theme-toggle i');
            if(body.getAttribute('data-theme') === 'light') {
                body.setAttribute('data-theme', 'dark');
                icon.className = 'fas fa-sun';
            } else {
                body.setAttribute('data-theme', 'light');
                icon.className = 'fas fa-moon';
            }
        }

        // Scroll Progress Logic
        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("scroll-progress").style.width = scrolled + "%";
        };
    </script>
</body>
</html>
