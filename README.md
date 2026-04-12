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
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* CEO Aura Background */
        .agency-aura { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(50%, 50%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 160px; }

        /* Live Global Notifications */
        #global-alert { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 92%; max-width: 440px; display: none; }
        .alert-ui { background: rgba(0, 0, 0, 0.95); border: 1px solid var(--primary); padding: 15px 25px; border-radius: 50px; backdrop-filter: blur(25px); display: flex; align-items: center; gap: 15px; box-shadow: 0 10px 40px rgba(0,242,254,0.4); animation: slideIn 0.5s ease; }

        /* Mega Header */
        .agency-header { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 25px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); padding: 6px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.3); margin-bottom: 20px; }
        .brand-name { font-size: 2.8rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        /* Future Tab System */
        .tabs-container { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-trigger { background: var(--glass); border: 1px solid var(--border); padding: 14px 28px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.85rem; transition: 0.3s; font-weight: 600; }
        .tab-trigger.active { background: var(--primary); color: #000; border-color: var(--primary); box-shadow: 0 0 20px rgba(0,242,254,0.3); }

        /* Content Sections */
        .view-pane { display: none; }
        .view-pane.active { display: block; animation: fadeInUp 0.5s ease; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

        /* Elite Feature Cards */
        .feature-card { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 20px; border-left: 5px solid transparent; transition: 0.3s; }
        .feature-card:hover { border-left-color: var(--primary); background: rgba(0,242,254,0.04); transform: scale(1.02); }
        .icon-p { font-size: 2rem; color: var(--primary); margin-bottom: 15px; }

        /* Pricing Calculator UI */
        .calc-box { background: rgba(0,242,254,0.05); border: 1px dashed var(--primary); border-radius: 30px; padding: 25px; text-align: center; margin-top: 20px; }
        
        /* Floating Bot */
        .ai-bot { position: fixed; bottom: 110px; right: 25px; width: 60px; height: 60px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.5rem; color: #000; cursor: pointer; box-shadow: 0 10px 30px rgba(0,242,254,0.5); z-index: 9998; animation: bounce 3s infinite; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(45px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; }
        .nav-icon { color: white; opacity: 0.35; font-size: 1.5rem; cursor: pointer; transition: 0.4s; }
        .nav-icon.active { opacity: 1; color: var(--primary); transform: translateY(-10px); }
        
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 25px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 1rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 20px; }
    </style>
</head>
<body>

    <div class="agency-aura"><div class="glow"></div></div>

    <div id="global-alert">
        <div class="alert-ui">
            <i class="fas fa-globe-americas" style="color: var(--primary);"></i>
            <span id="alert-txt" style="font-size: 0.8rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="ai-bot" onclick="navTo('contact', this)"><i class="fas fa-robot"></i></div>

    <div class="container">
        
        <header class="agency-header" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="Muhammad Nazim CEO">
            <div class="brand-name">PRIME SOLUTIONS</div>
            <p style="opacity: 0.6; font-size: 0.85rem; letter-spacing: 2px; font-weight: 300;">GLOBAL ENTERPRISE AGENCY</p>
            <div style="display: flex; justify-content: center; gap: 12px; margin-top: 30px;">
                <a href="https://wa.me/923332637235" class="tab-trigger active" style="text-decoration:none;">Partner With Us</a>
            </div>
        </header>

        <div class="tabs-container">
            <div class="tab-trigger active" onclick="navTo('home', this)">Agency</div>
            <div class="tab-trigger" onclick="navTo('solutions', this)">Our Solutions</div>
            <div class="tab-trigger" onclick="navTo('calculator', this)">Price Calc</div>
            <div class="tab-trigger" onclick="navTo('contact', this)">B2B Support</div>
        </div>

        <section id="pane-home" class="view-pane active">
            <div class="feature-card">
                <i class="fas fa-microchip icon-p"></i>
                <h3>Company Vision</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.8; margin-top: 15px;">
                    Muhammad Nazim ki sarbarahi mein Prime Solutions dunya ki leading agency hai. Hum high-end automation, AI integration, aur custom software development mein specialize karte hain.
                </p>
            </div>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                <div class="feature-card" style="text-align:center;"><h2>200+</h2><p style="font-size:0.6rem;">PROJECTS</p></div>
                <div class="feature-card" style="text-align:center;"><h2>100%</h2><p style="font-size:0.6rem;">SUCCESS</p></div>
            </div>
        </section>

        <section id="pane-solutions" class="view-pane">
            <div class="feature-card">
                <i class="fas fa-university icon-p"></i>
                <h4>Educational Ecosystems</h4>
                <p style="font-size: 0.75rem; opacity: 0.5;">Advanced ERP for Schools & Colleges.</p>
            </div>
            <div class="feature-card">
                <i class="fas fa-chart-line icon-p"></i>
                <h4>Fin-Tech Dashboards</h4>
                <p style="font-size: 0.75rem; opacity: 0.5;">Real-time ROI Tracking & Security.</p>
            </div>
            <div class="feature-card">
                <i class="fas fa-hospital-user icon-p"></i>
                <h4>Health-Care Portals</h4>
                <p style="font-size: 0.75rem; opacity: 0.5;">Doctor-Patient automated scheduling.</p>
            </div>
        </section>

        <section id="pane-calculator" class="view-pane">
            <div class="feature-card">
                <h3>Instant Project Quote</h3>
                <p style="font-size: 0.8rem; opacity: 0.5; margin-bottom: 20px;">Select your needs to see estimated pricing.</p>
                <div class="calc-box">
                    <p id="quote-display" style="font-size: 1.5rem; font-weight: 800; color: var(--primary);">$0.00</p>
                    <p style="font-size: 0.6rem; opacity: 0.5;">Estimated Start Price</p>
                </div>
                <button class="btn-action" onclick="alert('Redirecting to CEO for exact quote...')">Get Exact Price</button>
            </div>
        </section>

        <section id="pane-contact" class="view-pane">
            <div class="feature-card">
                <h3>Contact CEO HQ</h3>
                <input type="text" id="c-name" placeholder="Your Brand Name" style="width:100%; padding:20px; border-radius:20px; background:rgba(255,255,255,0.04); border:1px solid var(--border); color:white; margin-top:20px; outline:none;">
                <textarea id="c-msg" rows="3" placeholder="Project Requirements..." style="width:100%; padding:20px; border-radius:20px; background:rgba(255,255,255,0.04); border:1px solid var(--border); color:white; margin-top:15px; outline:none;"></textarea>
                <a href="javascript:void(0)" class="btn-action" onclick="sendInquiry()">
                    <i class="fab fa-whatsapp"></i> START CONSULTATION
                </a>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.2; font-size: 0.6rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL CONGLOMERATE © 2026<br>
            CHIEF EXECUTIVE OFFICER: MUHAMMAD NAZIM
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home', this)"><i class="fas fa-building"></i></div>
        <div class="nav-icon" onclick="navTo('solutions', this)"><i class="fas fa-rocket"></i></div>
        <div class="nav-icon" onclick="navTo('calculator', this)"><i class="fas fa-calculator"></i></div>
        <div class="nav-icon" onclick="navTo('contact', this)"><i class="fas fa-envelope-open-text"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Sales Alert Logic
        const clients = ["Sheikh Mansour", "Dr. Emily", "Zubair", "CEO Mark", "Sophia"];
        const cities = ["Dubai", "Singapore", "New York", "Karachi", "London"];
        const projects = ["School ERP", "Investment App", "E-Com Hub", "AI Portal"];

        function triggerGlobalAlert() {
            const c = clients[Math.floor(Math.random() * clients.length)];
            const ci = cities[Math.floor(Math.random() * cities.length)];
            const p = projects[Math.floor(Math.random() * projects.length)];
            
            document.getElementById('alert-txt').innerText = `${c} from ${ci} just hired Prime Solutions for a ${p}!`;
            const box = document.getElementById('global-alert');
            box.style.display = 'block';
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(triggerGlobalAlert, 15000);

        // Multi-View Navigation
        function navTo(paneId, btn) {
            document.querySelectorAll('.view-pane').forEach(p => p.classList.remove('active'));
            document.getElementById('pane-' + paneId).classList.add('active');
            
            document.querySelectorAll('.tab-trigger, .nav-icon').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            window.scrollTo(0,0);

            if(paneId === 'calculator') {
                runCalculator();
            }
        }

        // Fake Price Calculator Logic
        function runCalculator() {
            let price = 500;
            const interval = setInterval(() => {
                price += Math.floor(Math.random() * 50);
                document.getElementById('quote-display').innerText = '$' + price + '.00';
                if(price > 1200) clearInterval(interval);
            }, 50);
        }

        // WhatsApp Logic
        function sendInquiry() {
            const n = document.getElementById('c-name').value;
            const m = document.getElementById('c-msg').value;
            const text = `Greetings Prime Solutions HQ! I am ${n}. Requesting proposal for: ${m}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
