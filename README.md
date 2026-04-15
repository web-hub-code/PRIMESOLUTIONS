<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | CEO Muhammad Nazim</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb; --webhub: #6a1b9a;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        .agency-aura { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(50%, 50%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 160px; }

        .agency-header { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 25px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.2); margin-bottom: 15px; object-fit: cover; }
        .brand-name { font-size: 2.5rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        .social-row { display: flex; justify-content: center; gap: 20px; margin-top: 15px; }
        .social-link { color: white; font-size: 1.1rem; opacity: 0.5; transition: 0.3s; }
        .social-link:hover { opacity: 1; color: var(--primary); transform: scale(1.2); }

        .tabs-container { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-trigger { background: var(--glass); border: 1px solid var(--border); padding: 12px 24px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.8rem; transition: 0.3s; font-weight: 600; }
        .tab-trigger.active { background: var(--primary); color: #000; border-color: var(--primary); box-shadow: 0 0 15px rgba(0,242,254,0.3); }

        .view-pane { display: none; }
        .view-pane.active { display: block; animation: fadeInUp 0.5s ease; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }

        .feature-card { background: var(--glass); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 15px; transition: 0.3s; overflow: hidden; position: relative; }
        .card-img { width: 100%; height: 200px; object-fit: cover; border-radius: 20px; margin-bottom: 15px; border: 1px solid var(--border); }
        
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 16px; border-radius: 18px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 0.9rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 10px; }

        .contact-info { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.02); padding: 15px; border-radius: 20px; border: 1px solid var(--border); }
        .contact-info i { color: var(--primary); font-size: 1.2rem; }

        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 450px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(40px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 9999; }
        .nav-icon { color: white; opacity: 0.3; font-size: 1.4rem; cursor: pointer; transition: 0.4s; }
        .nav-icon.active { opacity: 1; color: var(--primary); transform: translateY(-8px); }
    </style>
</head>
<body>

    <div class="agency-aura"><div class="glow"></div></div>

    <div class="container">
        
        <header class="agency-header" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="Muhammad Nazim">
            <div class="brand-name">PRIME SOLUTIONS</div>
            <p style="opacity: 0.5; font-size: 0.75rem; letter-spacing: 2px;">GLOBAL IT ENTERPRISE AGENCY</p>
            
            <div class="social-row">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-link"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-link"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                <a href="https://youtube.com/@crazykhantv" target="_blank" class="social-link"><i class="fab fa-youtube"></i></a>
            </div>
        </header>

        <div class="tabs-container">
            <div class="tab-trigger active" onclick="navTo('home', this)">Agency</div>
            <div class="tab-trigger" onclick="navTo('works', this)">Portfolio</div>
            <div class="tab-trigger" onclick="navTo('contact', this)">Contact HQ</div>
            <div class="tab-trigger" onclick="navTo('calculator', this)">Price Calc</div>
        </div>

        <section id="pane-home" class="view-pane active">
            <div class="feature-card">
                <h3 style="color:var(--primary); margin-bottom:10px;">Executive Summary</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.7;">
                    Prime Solutions provides elite-level software development, financial automation, and digital branding. Led by Muhammad Nazim, we turn complex ideas into global realities.
                </p>
                <a href="https://wa.me/923332637235" class="btn-action">Start WhatsApp Chat <i class="fab fa-whatsapp"></i></a>
            </div>
        </section>

        <section id="pane-works" class="view-pane">
            <div class="feature-card" style="padding:15px;">
                <img src="Screenshot_2026-04-15-10-11-35-44.png" class="card-img">
                <h4 style="color:var(--webhub)">WebHub Dashboard</h4>
                <a href="https://web-hub-code.github.io/Web-hub/" target="_blank" class="btn-action" style="padding:12px;">Live Demo</a>
            </div>
            <div class="feature-card" style="padding:15px;">
                <img src="Screenshot_2026-04-15-10-04-08-81.png" class="card-img">
                <h4 style="color:#ffd700">MintCrestGold</h4>
                <a href="https://gtv140.github.io/investment/" target="_blank" class="btn-action" style="padding:12px; background:linear-gradient(45deg,#ffd700,#ffb300)">Visit Vault</a>
            </div>
        </section>

        <section id="pane-contact" class="view-pane">
            <div class="feature-card">
                <h3 style="margin-bottom:20px;">Get In Touch</h3>
                
                <div class="contact-info">
                    <i class="fas fa-phone-alt"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">DIRECT CALL</p>
                        <a href="tel:03705519562" style="color:white; text-decoration:none; font-weight:600;">03705519562</a>
                    </div>
                </div>

                <div class="contact-info">
                    <i class="fab fa-whatsapp"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">WHATSAPP ONLY</p>
                        <a href="https://wa.me/923332637235" style="color:white; text-decoration:none; font-weight:600;">03332637235</a>
                    </div>
                </div>

                <div class="contact-info">
                    <i class="fas fa-envelope"></i>
                    <div>
                        <p style="font-size:0.6rem; opacity:0.5;">OFFICIAL EMAIL</p>
                        <a href="mailto:webhub262@gmail.com" style="color:white; text-decoration:none; font-weight:600;">webhub262@gmail.com</a>
                    </div>
                </div>

                <button class="btn-action" onclick="window.location.href='mailto:webhub262@gmail.com'">Send Quick Inquiry</button>
            </div>
        </section>

        <section id="pane-calculator" class="view-pane">
            <div class="feature-card">
                <h3>Price Estimator</h3>
                <div style="background:rgba(0,242,254,0.05); border:1px dashed var(--primary); padding:25px; border-radius:20px; text-align:center; margin:20px 0;">
                    <p id="quote-display" style="font-size:2rem; font-weight:800; color:var(--primary);">$0.00</p>
                </div>
                <button class="btn-action" onclick="navTo('contact', document.querySelectorAll('.nav-icon')[2])">Request Official Quote</button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.2; font-size: 0.6rem;">
            PRIME SOLUTIONS © 2026 | MUHAMMAD NAZIM
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home', this)"><i class="fas fa-home"></i></div>
        <div class="nav-icon" onclick="navTo('works', this)"><i class="fas fa-briefcase"></i></div>
        <div class="nav-icon" onclick="navTo('contact', this)"><i class="fas fa-address-book"></i></div>
        <div class="nav-icon" onclick="navTo('calculator', this)"><i class="fas fa-calculator"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });
        function navTo(paneId, btn) {
            document.querySelectorAll('.view-pane').forEach(p => p.classList.remove('active'));
            document.getElementById('pane-' + paneId).classList.add('active');
            document.querySelectorAll('.tab-trigger, .nav-icon').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            window.scrollTo(0,0);
            if(paneId === 'calculator') runCalculator();
        }
        function runCalculator() {
            let price = 500;
            const target = 1500 + Math.floor(Math.random() * 500);
            const interval = setInterval(() => {
                price += 43;
                document.getElementById('quote-display').innerText = '$' + price + '.00';
                if(price >= target) clearInterval(interval);
            }, 30);
        }
    </script>
</body>
</html>
