<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | World's #1 Digital Agency</title>
    
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

        /* Infinity Background */
        .hero-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; 
            background: url('https://images.unsplash.com/photo-1451187580459-43490279c0fa?auto=format&fit=crop&q=80') center/cover; filter: brightness(0.2); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 150px; }

        /* Fake Notifications */
        #notify-box { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 85%; max-width: 400px; display: none; }
        .notify { background: rgba(0, 0, 0, 0.9); border: 1px solid var(--primary); padding: 15px; border-radius: 20px; backdrop-filter: blur(10px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 30px rgba(0,242,254,0.2); animation: slideDown 0.5s forwards; }
        @keyframes slideDown { from { transform: translateY(-50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        /* Glass Cards */
        .glass-card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 40px; padding: 30px; margin-bottom: 25px; transition: 0.4s; }
        .glass-card:hover { border-color: var(--primary); transform: translateY(-5px); }

        /* CEO Profile */
        .pfp-wrap { position: relative; width: 140px; height: 140px; margin: 0 auto 20px; }
        .pfp-img { width: 100%; height: 100%; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; object-fit: cover; }
        .online-tag { position: absolute; bottom: 10px; right: 10px; background: #25d366; width: 15px; height: 15px; border-radius: 50%; border: 3px solid #000; box-shadow: 0 0 10px #25d366; }

        /* Social Icons */
        .social-dock { display: flex; justify-content: center; gap: 15px; margin-top: 20px; }
        .social-item { width: 45px; height: 45px; background: var(--glass); border-radius: 15px; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; color: white; text-decoration: none; border: 1px solid var(--border); transition: 0.3s; }
        .social-item:hover { color: var(--primary); border-color: var(--primary); transform: scale(1.1); }

        /* Modern Services */
        .service-link { display: flex; align-items: center; gap: 15px; padding: 18px; background: rgba(255,255,255,0.02); border-radius: 22px; margin-bottom: 15px; text-decoration: none; color: white; border: 1px solid transparent; }
        .service-link:hover { border-color: var(--primary); background: rgba(0,242,254,0.05); }

        /* Reviews */
        .review-box { margin-top: 20px; }
        .rev-item { background: rgba(255,255,255,0.02); padding: 15px; border-radius: 20px; margin-bottom: 10px; font-size: 0.8rem; }
        .stars { color: #f1c40f; margin-bottom: 5px; }

        /* Tabs/Nav */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 450px; background: rgba(0,0,0,0.9); backdrop-filter: blur(25px); border-radius: 50px; display: flex; justify-content: space-around; padding: 18px; border: 1px solid var(--border); z-index: 9999; }
        .nav-icon { color: white; opacity: 0.4; font-size: 1.3rem; cursor: pointer; }
        .nav-icon.active { color: var(--primary); opacity: 1; }

        .section-view { display: none; }
        .section-view.active { display: block; animation: fadeIn 0.5s; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; border: none; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 20px; text-decoration: none; }
    </style>
</head>
<body>

    <div class="hero-bg"></div>

    <div id="notify-box">
        <div class="notify">
            <i class="fas fa-check-circle" style="color: var(--primary);"></i>
            <span id="notify-text" style="font-size: 0.7rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        <section id="view-home" class="section-view active">
            <div class="glass-card" style="text-align: center;" data-aos="fade-down">
                <div class="pfp-wrap">
                    <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-img" alt="CEO">
                    <div class="online-tag"></div>
                </div>
                <h1 style="font-size: 2.5rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
                <p style="opacity: 0.7; font-size: 0.9rem;">Global CEO & Architect of Prime Solutions</p>
                
                <div class="social-dock">
                    <a href="#" class="social-item"><i class="fab fa-facebook-f"></i></a>
                    <a href="#" class="social-item"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="social-item"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" class="social-item"><i class="fab fa-github"></i></a>
                </div>
            </div>

            <div class="glass-card" data-aos="fade-up">
                <h3><i class="fas fa-chart-line" style="color: var(--primary);"></i> Global Performance</h3>
                <div style="display: flex; justify-content: space-around; margin-top: 20px; text-align: center;">
                    <div><h2 style="color: var(--primary);">150+</h2><p style="font-size: 0.6rem; opacity: 0.5;">PROJECTS</p></div>
                    <div><h2 style="color: var(--primary);">50+</h2><p style="font-size: 0.6rem; opacity: 0.5;">CLIENTS</p></div>
                    <div><h2 style="color: var(--primary);">5.0</h2><p style="font-size: 0.6rem; opacity: 0.5;">RATING</p></div>
                </div>
            </div>
        </section>

        <section id="view-services" class="section-view">
            <div class="glass-card">
                <h3 style="margin-bottom: 20px;">Elite Services</h3>
                <a href="#contact" class="service-link" onclick="navTo('contact')">
                    <i class="fas fa-wallet"></i>
                    <div><h4>Investment Systems</h4><p style="font-size: 0.6rem; opacity: 0.5;">Safe & high-speed profit tracking portals.</p></div>
                </a>
                <a href="#contact" class="service-link" onclick="navTo('contact')">
                    <i class="fas fa-shopping-bag"></i>
                    <div><h4>Premium E-Commerce</h4><p style="font-size: 0.6rem; opacity: 0.5;">Modern stores with global payment gateways.</p></div>
                </a>
                <a href="#contact" class="service-link" onclick="navTo('contact')">
                    <i class="fas fa-robot"></i>
                    <div><h4>AI & Automation</h4><p style="font-size: 0.6rem; opacity: 0.5;">Smart bots and business automation tools.</p></div>
                </a>
            </div>
        </section>

        <section id="view-trust" class="section-view">
            <div class="glass-card">
                <h3>Global Feedback</h3>
                <div class="review-box">
                    <div class="rev-item">
                        <div class="stars">★★★★★</div>
                        <p><b>John D. (USA):</b> "Best experience! Nazim delivered my project before time. 100% recommended."</p>
                    </div>
                    <div class="rev-item">
                        <div class="stars">★★★★★</div>
                        <p><b>Sarah K. (UK):</b> "The investment portal is so smooth. High quality work by Prime Solutions."</p>
                    </div>
                    <div class="rev-item">
                        <div class="stars">★★★★★</div>
                        <p><b>Ahmed R. (UAE):</b> "Top class service. Best developer in the market right now."</p>
                    </div>
                </div>
            </div>
            
            <div class="glass-card">
                <h3><i class="fas fa-user-lock"></i> Privacy Policy</h3>
                <p style="font-size: 0.7rem; opacity: 0.6; line-height: 1.6; margin-top: 10px;">
                    Prime Solutions is committed to your security. We use end-to-end encryption for all data. Your project ideas and financial data are protected under strict NDA (Non-Disclosure Agreement). We never share your data with third parties.
                </p>
            </div>
        </section>

        <section id="view-contact" class="section-view">
            <div class="glass-card">
                <h3>Start a Collaboration</h3>
                <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 20px;">Fill details to connect with CEO Nazim.</p>
                <input type="text" id="nameInp" placeholder="Your Name" style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
                <textarea id="msgInp" rows="3" placeholder="Project details..." style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 20px; outline: none;"></textarea>
                
                <a href="javascript:void(0)" class="btn-main" onclick="sendToCEO()">
                    <i class="fab fa-whatsapp"></i> MESSAGE CEO NAZIM
                </a>
                <a href="tel:03705519562" class="btn-main" style="background: transparent; border: 1px solid var(--primary); color: var(--primary);">
                    <i class="fas fa-phone"></i> CALL: 0370 5519562
                </a>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 30px; opacity: 0.3; font-size: 0.7rem;">
            © 2026 PRIME SOLUTIONS | WORLD'S #1 AGENCY<br>
            HEADQUARTERS: PAKISTAN | GLOBAL SERVICE
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home')"><i class="fas fa-house"></i></div>
        <div class="nav-icon" onclick="navTo('services')"><i class="fas fa-th-large"></i></div>
        <div class="nav-icon" onclick="navTo('trust')"><i class="fas fa-shield-check"></i></div>
        <div class="nav-icon" onclick="navTo('contact')"><i class="fas fa-paper-plane"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Fake Notifications Logic
        const users = ["Ali R.", "James M.", "Fatima", "Chen Wei", "Sofia", "David L."];
        const locations = ["London", "Dubai", "New York", "Karachi", "Singapore"];
        const projects = ["Investment Site", "E-Commerce App", "Portfolio", "SEO Strategy"];

        function showNotify() {
            const user = users[Math.floor(Math.random() * users.length)];
            const loc = locations[Math.floor(Math.random() * locations.length)];
            const proj = projects[Math.floor(Math.random() * projects.length)];
            
            document.getElementById('notify-text').innerText = `${user} from ${loc} just ordered a ${proj}!`;
            const box = document.getElementById('notify-box');
            box.style.display = 'block';
            
            setTimeout(() => { box.style.display = 'none'; }, 4000);
        }
        setInterval(showNotify, 8000);

        // Page Navigation
        function navTo(pageId) {
            document.querySelectorAll('.section-view').forEach(s => s.classList.remove('active'));
            document.getElementById('view-' + pageId).classList.add('active');
            
            document.querySelectorAll('.nav-icon').forEach(i => i.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        // WhatsApp Logic
        function sendToCEO() {
            const name = document.getElementById('nameInp').value;
            const msg = document.getElementById('msgInp').value;
            const text = `Hello CEO Nazim! I am ${name}. Project vision: ${msg}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
