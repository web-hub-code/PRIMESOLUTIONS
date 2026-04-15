<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | Global IT Enterprise & Agency</title>
    
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

        /* CEO Aura Background */
        .agency-aura { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(50%, 50%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 160px; }

        /* Header UI */
        .agency-header { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 25px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); padding: 6px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.3); margin-bottom: 20px; object-fit: cover; }
        .brand-name { font-size: 2.8rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        /* Tab System */
        .tabs-container { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-trigger { background: var(--glass); border: 1px solid var(--border); padding: 14px 28px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.85rem; transition: 0.3s; font-weight: 600; }
        .tab-trigger.active { background: var(--primary); color: #000; border-color: var(--primary); box-shadow: 0 0 20px rgba(0,242,254,0.3); }

        /* Panes */
        .view-pane { display: none; }
        .view-pane.active { display: block; animation: fadeInUp 0.5s ease; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

        /* Project Cards */
        .feature-card { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 20px; transition: 0.3s; overflow: hidden; }
        .feature-card:hover { transform: scale(1.02); background: rgba(0,242,254,0.06); border-color: var(--primary); }
        .card-img { width: 100%; height: 220px; object-fit: cover; border-bottom: 1px solid var(--border); }
        
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; border-radius: 20px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 0.9rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 15px; transition: 0.3s; }
        .btn-action:hover { opacity: 0.9; transform: translateY(-2px); box-shadow: 0 5px 15px rgba(0,242,254,0.3); }

        /* Pricing UI */
        .calc-box { background: rgba(0,242,254,0.05); border: 1px dashed var(--primary); border-radius: 30px; padding: 25px; text-align: center; margin-top: 20px; }

        /* Nav */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(45px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; }
        .nav-icon { color: white; opacity: 0.35; font-size: 1.5rem; cursor: pointer; transition: 0.4s; }
        .nav-icon.active { opacity: 1; color: var(--primary); transform: translateY(-10px); }
    </style>
</head>
<body>

    <div class="agency-aura"><div class="glow"></div></div>

    <div class="container">
        
        <header class="agency-header" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="Muhammad Nazim CEO">
            <div class="brand-name">PRIME SOLUTIONS</div>
            <p style="opacity: 0.6; font-size: 0.85rem; letter-spacing: 2px; font-weight: 300;">GLOBAL ENTERPRISE AGENCY</p>
        </header>

        <div class="tabs-container">
            <div class="tab-trigger active" onclick="navTo('home', this)">Agency</div>
            <div class="tab-trigger" onclick="navTo('works', this)">Portfolio Hub</div>
            <div class="tab-trigger" onclick="navTo('solutions', this)">Solutions</div>
            <div class="tab-trigger" onclick="navTo('calculator', this)">Price Calc</div>
        </div>

        <section id="pane-home" class="view-pane active">
            <div class="feature-card" data-aos="fade-up">
                <i class="fas fa-microchip" style="font-size: 2rem; color: var(--primary); margin-bottom:15px;"></i>
                <h3>CEO HQ Vision</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.8; margin-top: 10px;">
                    Under the expert leadership of Muhammad Nazim, Prime Solutions is redefining global tech standards. We specialize in AI, high-end web architecture, and secure financial ecosystems.
                </p>
            </div>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                <div class="feature-card" style="text-align:center;"><h2>200+</h2><p style="font-size:0.6rem;">DEPLOYMENTS</p></div>
                <div class="feature-card" style="text-align:center;"><h2>100%</h2><p style="font-size:0.6rem;">SATISFACTION</p></div>
            </div>
        </section>

        <section id="pane-works" class="view-pane">
            
            <div class="feature-card" style="padding:0; border: 2px solid var(--webhub);">
                <img src="Screenshot_2026-04-15-10-11-35-44.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:var(--webhub)">WebHub Command</h4>
                    <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">Centralized management hub for interconnected digital services.</p>
                    <a href="https://web-hub-code.github.io/Web-hub/" target="_blank" class="btn-action">Live Deployment <i class="fas fa-external-link-alt"></i></a>
                </div>
            </div>

            <div class="feature-card" style="padding:0; border-bottom: 4px solid #ffd700;">
                <img src="Screenshot_2026-04-15-10-04-08-81.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:#ffd700">MintCrestGold</h4>
                    <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">High-end investment dashboard for real-time gold asset tracking.</p>
                    <a href="https://gtv140.github.io/investment/" target="_blank" class="btn-action" style="background:linear-gradient(45deg, #ffd700, #ffb300)">Access Vault <i class="fas fa-coins"></i></a>
                </div>
            </div>

            <div class="feature-card" style="padding:0; border-bottom: 4px solid var(--secondary);">
                <img src="Screenshot_2026-04-15-09-59-25-00.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:var(--secondary)">Live Connect</h4>
                    <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">Real-time communication suite for professional enterprises.</p>
                    <a href="https://gtv140.github.io/Live-chat/" target="_blank" class="btn-action">Join Chat <i class="fas fa-comments"></i></a>
                </div>
            </div>

            <div class="feature-card" style="padding:0; border-bottom: 4px solid var(--accent);">
                <img src="Screenshot_2026-04-15-10-01-13-43.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:var(--accent)">Prime Academy</h4>
                    <p style="font-size:0.75rem; opacity:0.6; margin-bottom:15px;">Futuristic e-learning portal for digital education excellence.</p>
                    <button class="btn-action" style="opacity:0.5; cursor:not-allowed;">Launching Soon <i class="fas fa-hourglass-half"></i></button>
                </div>
            </div>

        </section>

        <section id="pane-solutions" class="view-pane">
            <div class="feature-card">
                <i class="fas fa-rocket icon-p" style="color:var(--primary); font-size:2rem;"></i>
                <h3 style="margin-top:10px;">Enterprise Solutions</h3>
                <p style="font-size:0.8rem; opacity:0.5; margin-top:10px;">Custom CRM, ERP, and AI systems tailored for your brand's growth.</p>
            </div>
            <div class="feature-card">
                <i class="fas fa-shield-alt icon-p" style="color:var(--accent); font-size:2rem;"></i>
                <h3 style="margin-top:10px;">Security First</h3>
                <p style="font-size:0.8rem; opacity:0.5; margin-top:10px;">SSL encryption and blockchain-verified transaction security.</p>
            </div>
        </section>

        <section id="pane-calculator" class="view-pane">
            <div class="feature-card">
                <h3>Global Project Quote</h3>
                <div class="calc-box"><p id="quote-display" style="font-size: 2rem; font-weight: 800; color: var(--primary);">$0.00</p></div>
                <p style="text-align:center; font-size:0.6rem; opacity:0.4; margin-top:10px;">*Price varies based on API requirements.</p>
                <button class="btn-action" onclick="window.location.href='https://wa.me/923332637235'">Consult CEO For Exact Price</button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.3; font-size: 0.6rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL ENTERPRISE © 2026<br>
            CHIEF EXECUTIVE OFFICER: MUHAMMAD NAZIM
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home', this)"><i class="fas fa-university"></i></div>
        <div class="nav-icon" onclick="navTo('works', this)"><i class="fas fa-layer-group"></i></div>
        <div class="nav-icon" onclick="navTo('solutions', this)"><i class="fas fa-rocket"></i></div>
        <div class="nav-icon" onclick="navTo('calculator', this)"><i class="fas fa-calculator"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        // Initialize AOS
        AOS.init({ duration: 800, once: true });

        // Navigation Logic
        function navTo(paneId, btn) {
            document.querySelectorAll('.view-pane').forEach(p => p.classList.remove('active'));
            document.getElementById('pane-' + paneId).classList.add('active');
            
            document.querySelectorAll('.tab-trigger, .nav-icon').forEach(b => b.classList.remove('active'));
            
            // Syncing both tab and icon active states
            btn.classList.add('active');
            window.scrollTo(0,0);

            if(paneId === 'calculator') runCalculator();
        }

        // Live Price Generator
        function runCalculator() {
            let price = 500;
            const target = 1500 + Math.floor(Math.random() * 1000);
            const interval = setInterval(() => {
                price += 43;
                document.getElementById('quote-display').innerText = '$' + price + '.00';
                if(price >= target) clearInterval(interval);
            }, 30);
        }
    </script>
</body>
</html>
