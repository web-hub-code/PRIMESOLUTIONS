<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    
    <title>Prime Solutions | Premier Web Architecture & IT Agency by M Nazim</title>
    <meta name="description" content="Prime Solutions by Muhammad Nazim provides high-end web development, AI automation, and secure Fintech systems. Expert IT solutions for global enterprises.">
    <meta name="keywords" content="Prime Solutions, Muhammad Nazim, Web Developer Pakistan, Software Agency, AI Automation, Fintech Development, Custom Web Architecture, IT Solutions">
    <meta name="author" content="Muhammad Nazim">
    
    <meta property="og:title" content="Prime Solutions | Digital Excellence by M Nazim">
    <meta property="og:description" content="Transforming complex ideas into scalable digital realities. Explore our portfolio.">
    <meta property="og:url" content="https://web-hub-code.github.io/PRIMESOLUTIONS/">
    <meta property="og:image" content="Screenshot_2026-04-12-10-02-54-39.png">
    <meta property="og:type" content="website">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb; --webhub: #6a1b9a;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
            --gold: #ffd700;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; line-height: 1.6; }

        /* CEO Aura Background */
        .agency-aura { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(50%, 50%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 160px; }

        /* Mega Header */
        .agency-header { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 40px 20px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.2); margin-bottom: 15px; object-fit: cover; }
        .brand-name { font-size: 2.5rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; margin-bottom: 5px; }
        
        .social-row { display: flex; justify-content: center; gap: 20px; margin-top: 15px; }
        .social-link { color: white; font-size: 1.2rem; opacity: 0.5; transition: 0.3s; }
        .social-link:hover { opacity: 1; color: var(--primary); transform: translateY(-3px); }

        /* Tabs System */
        .tabs-container { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-trigger { background: var(--glass); border: 1px solid var(--border); padding: 12px 24px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.8rem; transition: 0.3s; font-weight: 600; }
        .tab-trigger.active { background: var(--primary); color: #000; border-color: var(--primary); box-shadow: 0 0 15px rgba(0,242,254,0.3); }

        /* View Panes */
        .view-pane { display: none; }
        .view-pane.active { display: block; animation: fadeInUp 0.5s ease; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }

        /* Cards Style */
        .feature-card { background: var(--glass); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 15px; transition: 0.3s; overflow: hidden; }
        .card-img { width: 100%; height: 210px; object-fit: cover; border-radius: 20px; margin-bottom: 15px; border: 1px solid var(--border); }
        
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 16px; border-radius: 18px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 0.9rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 10px; transition: 0.3s; }
        .btn-action:hover { transform: scale(1.02); box-shadow: 0 5px 15px rgba(0,242,254,0.3); }

        .contact-info { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.02); padding: 15px; border-radius: 20px; border: 1px solid var(--border); }
        .contact-info i { color: var(--primary); font-size: 1.2rem; }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 450px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(40px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 9999; }
        .nav-icon { color: white; opacity: 0.3; font-size: 1.4rem; cursor: pointer; transition: 0.4s; }
        .nav-icon.active { opacity: 1; color: var(--primary); transform: translateY(-8px); }

        .tag-badge { font-size: 0.65rem; background: var(--primary); color: #000; padding: 4px 10px; border-radius: 10px; font-weight: 800; display: inline-block; margin-bottom: 10px; }
    </style>
</head>
<body>

    <div class="agency-aura"><div class="glow"></div></div>

    <div class="container">
        
        <header class="agency-header" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="Muhammad Nazim CEO of Prime Solutions">
            <h1 class="brand-name">PRIME SOLUTIONS</h1>
            <p style="opacity: 0.5; font-size: 0.75rem; letter-spacing: 2px;">GLOBAL IT ENTERPRISE AGENCY</p>
            
            <div class="social-row">
                <a href="https://www.facebook.com/profile.php?id=61590925586953" target="_blank" class="social-link" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-link" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-link" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                <a href="https://youtube.com/@crazykhantv" target="_blank" class="social-link" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
            </div>
        </header>

        <div class="tabs-container">
            <div class="tab-trigger active" onclick="navTo('home', this)">Agency Vision</div>
            <div class="tab-trigger" onclick="navTo('works', this)">Portfolio Hub</div>
            <div class="tab-trigger" onclick="navTo('contact', this)">Contact HQ</div>
            <div class="tab-trigger" onclick="navTo('calculator', this)">Project Estimator</div>
        </div>

        <section id="pane-home" class="view-pane active">
            <div class="feature-card" data-aos="fade-up">
                <span class="tag-badge">EXECUTIVE STATEMENT</span>
                <h2 style="color:var(--primary); margin-bottom:15px; font-size: 1.5rem;">Leading the Digital Frontier</h2>
                <p style="font-size: 0.85rem; opacity: 0.7; line-height: 1.8; margin-bottom: 15px;">
                    Under the leadership of <strong>Muhammad Nazim</strong>, Prime Solutions has emerged as a premier <strong>Global IT Enterprise Agency</strong>. We specialize in building high-performance <strong>custom web architectures</strong>, AI-integrated systems, and scalable digital products for modern businesses.
                </p>
                <p style="font-size: 0.85rem; opacity: 0.7; line-height: 1.8;">
                    Our expertise lies in bridging the gap between imagination and execution. Whether it is secure Fintech systems like ROI trackers or real-time communication suites, we ensure <strong>technical excellence</strong> and measurable market growth.
                </p>
                <a href="https://wa.me/923332637235" class="btn-action">Direct Strategy Call <i class="fab fa-whatsapp"></i></a>
            </div>
            
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                <div class="feature-card" style="text-align:center; padding:20px;">
                    <h2 style="color:var(--primary)">50+</h2>
                    <p style="font-size:0.6rem; opacity:0.5; font-weight:800;">GLOBAL PROJECTS</p>
                </div>
                <div class="feature-card" style="text-align:center; padding:20px;">
                    <h2 style="color:var(--accent)">A+</h2>
                    <p style="font-size:0.6rem; opacity:0.5; font-weight:800;">UX PERFORMANCE</p>
                </div>
            </div>
        </section>

        <section id="pane-works" class="view-pane">
            
            <div class="feature-card" style="border: 1px solid var(--webhub);" data-aos="fade-up">
                <img src="Screenshot_2026-04-15-10-11-35-44.png" class="card-img" alt="WebHub Digital Dashboard">
                <h3 style="color:var(--webhub)">WebHub Command Center</h3>
                <p style="font-size:0.75rem; opacity:0.8; margin-bottom:8px;"><strong>Domain:</strong> Asset Management & Automation</p>
                <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">A centralized enterprise dashboard for monitoring digital assets with real-time API sync and performance analytics.</p>
                <a href="https://web-hub-code.github.io/Web-hub/" target="_blank" class="btn-action">Explore WebHub</a>
            </div>

            <div class="feature-card" style="border-bottom: 4px solid var(--gold);" data-aos="fade-up">
                <img src="Screenshot_2026-04-15-10-04-08-81.png" class="card-img" alt="MintCrestGold Fintech App">
                <h3 style="color:var(--gold)">MintCrestGold Platform</h3>
                <p style="font-size:0.75rem; opacity:0.8; margin-bottom:8px;"><strong>Domain:</strong> Fintech & Secure ROI Tracking</p>
                <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">Luxury-grade investment system with automated dividend tracking and high-security transaction protocols.</p>
                <a href="https://gtv140.github.io/investment/" target="_blank" class="btn-action" style="background:linear-gradient(45deg,var(--gold),#b8860b)">Access Investment Vault</a>
            </div>

            <div class="feature-card" style="border-bottom: 4px solid var(--secondary);" data-aos="fade-up">
                <img src="Screenshot_2026-04-15-09-59-25-00.png" class="card-img" alt="Live Connect Chat Application">
                <h3 style="color:var(--secondary)">Live Connect Suite</h3>
                <p style="font-size:0.75rem; opacity:0.8; margin-bottom:8px;"><strong>Domain:</strong> Real-time WebSocket Messaging</p>
                <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">Zero-latency communication system built for corporate networking and real-time data exchange.</p>
                <a href="https://gtv140.github.io/Live-chat/" target="_blank" class="btn-action">Join Corporate Network</a>
            </div>

        </section>

        <section id="pane-contact" class="view-pane">
            <div class="feature-card" data-aos="fade-up">
                <h2 style="margin-bottom:20px; font-size: 1.5rem;">Corporate Channels</h2>
                
                <div class="contact-info">
                    <i class="fas fa-phone-alt"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">EXECUTIVE LINE</p>
                        <a href="tel:03705519562" style="color:white; text-decoration:none; font-weight:600;">0370 5519562</a>
                    </div>
                </div>

                <div class="contact-info">
                    <i class="fab fa-whatsapp"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">WHATSAPP SUPPORT</p>
                        <a href="https://wa.me/923379827882" style="color:white; text-decoration:none; font-weight:600;">0337 9827882</a>
                    </div>
                </div>

                <div class="contact-info">
                    <i class="fas fa-envelope"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">OFFICIAL EMAIL</p>
                        <a href="mailto:webhub262@gmail.com" style="color:white; text-decoration:none; font-weight:600;">webhub262@gmail.com</a>
                    </div>
                </div>

                <button class="btn-action" onclick="window.location.href='mailto:webhub262@gmail.com'">Email Headquarters</button>
            </div>
        </section>

        <section id="pane-calculator" class="view-pane">
            <div class="feature-card" data-aos="fade-up">
                <h2 style="font-size: 1.5rem; margin-bottom: 10px;">Project Value Estimator</h2>
                <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 20px;">AI-calculated baseline for custom web & enterprise solutions.</p>
                
                <div style="background:rgba(0,242,254,0.05); border:1px dashed var(--primary); padding:30px; border-radius:25px; text-align:center; margin-bottom:20px;">
                    <p style="font-size: 0.6rem; letter-spacing: 2px; opacity: 0.5;">ESTIMATED STARTING COST</p>
                    <p id="quote-display" style="font-size:2.5rem; font-weight:800; color:var(--primary);">$0.00</p>
                </div>
                
                <p style="font-size: 0.7rem; opacity: 0.5; text-align: center; margin-bottom: 15px;">*Note: Final pricing depends on specific technical requirements and architecture scope.</p>
                <button class="btn-action" onclick="navTo('contact', document.querySelectorAll('.nav-icon')[2])">Get Official Quote</button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.2; font-size: 0.6rem; letter-spacing: 1px;">
            PRIME SOLUTIONS GLOBAL &copy; 2026 | DESIGNED BY M NAZIM ENTERPRISE
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home', this)" title="Home"><i class="fas fa-university"></i></div>
        <div class="nav-icon" onclick="navTo('works', this)" title="Portfolio"><i class="fas fa-briefcase"></i></div>
        <div class="nav-icon" onclick="navTo('contact', this)" title="Contact"><i class="fas fa-address-book"></i></div>
        <div class="nav-icon" onclick="navTo('calculator', this)" title="Price"><i class="fas fa-calculator"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });
        
        function navTo(paneId, btn) {
            // Hide all panes
            document.querySelectorAll('.view-pane').forEach(p => p.classList.remove('active'));
            // Show selected pane
            const targetPane = document.getElementById('pane-' + paneId);
            targetPane.classList.add('active');
            
            // Handle Navigation Highlights
            document.querySelectorAll('.tab-trigger, .nav-icon').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            
            // Sync bottom nav with top tabs
            const navIcons = document.querySelectorAll('.nav-icon');
            const tabTriggers = document.querySelectorAll('.tab-trigger');
            
            if(paneId === 'home') { navIcons[0].classList.add('active'); tabTriggers[0].classList.add('active'); }
            if(paneId === 'works') { navIcons[1].classList.add('active'); tabTriggers[1].classList.add('active'); }
            if(paneId === 'contact') { navIcons[2].classList.add('active'); tabTriggers[2].classList.add('active'); }
            if(paneId === 'calculator') { navIcons[3].classList.add('active'); tabTriggers[3].classList.add('active'); runCalculator(); }
            
            window.scrollTo(0,0);
        }

        function runCalculator() {
            let price = 500;
            const target = 1800 + Math.floor(Math.random() * 700);
            const interval = setInterval(() => {
                price += 57;
                document.getElementById('quote-display').innerText = '$' + price + '.00';
                if(price >= target) {
                    document.getElementById('quote-display').innerText = '$' + target + '.00';
                    clearInterval(interval);
                }
            }, 30);
        }
    </script>
</body>
</html>
