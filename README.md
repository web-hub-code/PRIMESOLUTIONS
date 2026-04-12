<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Founder & Owner Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #fdfdfd; --text: #1d1d1f; --glass: rgba(255, 255, 255, 0.8); --border: rgba(0, 0, 0, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        .bg-canvas { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 0% 0%, #e0f7fa 0%, #ffffff 50%, #f3e5f5 100%); }
        #progress-bar { position: fixed; top: 0; left: 0; width: 0%; height: 4px; background: linear-gradient(to right, var(--primary), var(--accent)); z-index: 9999; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 40px 15px 120px; }

        /* Premium Luxury Card System */
        .card { 
            background: var(--glass); backdrop-filter: blur(25px); -webkit-backdrop-filter: blur(25px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 40px rgba(0,0,0,0.04);
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 25px 50px rgba(79, 172, 254, 0.12); }

        /* Hero Styling */
        .hero { text-align: center; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid #fff; box-shadow: 0 15px 35px rgba(0,0,0,0.1); margin-bottom: 20px; }
        .gradient-text { background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; letter-spacing: -1px; }
        
        /* Interactive Stats */
        .stats-row { display: flex; justify-content: space-between; margin-top: 30px; border-top: 1px solid var(--border); padding-top: 20px; }
        .stat-box h2 { color: var(--primary); font-size: 1.6rem; font-weight: 800; }
        .stat-box p { font-size: 0.6rem; text-transform: uppercase; letter-spacing: 1.5px; opacity: 0.5; }

        /* Skill Bars */
        .skill-box { margin-bottom: 15px; }
        .skill-info { display: flex; justify-content: space-between; font-size: 0.75rem; margin-bottom: 5px; font-weight: 600; }
        .bar-bg { background: rgba(0,0,0,0.05); height: 8px; border-radius: 10px; }
        .bar-fill { height: 100%; border-radius: 10px; background: linear-gradient(to right, var(--primary), var(--secondary)); box-shadow: 0 0 10px rgba(79, 172, 254, 0.3); }

        /* Service Badges */
        .badge-container { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 15px; }
        .badge { background: #f0f3f6; color: #444; padding: 8px 16px; border-radius: 50px; font-size: 0.75rem; font-weight: 600; border: 1px solid var(--border); transition: 0.3s; }
        .badge:hover { background: var(--primary); color: white; }

        /* Multi-Step Process */
        .step { display: flex; gap: 15px; margin-bottom: 20px; }
        .step-num { min-width: 32px; height: 32px; border-radius: 50%; background: var(--primary); color: white; display: flex; align-items: center; justify-content: center; font-weight: 800; font-size: 0.9rem; }

        /* Professional Buttons */
        .btn-action { display: flex; align-items: center; justify-content: center; gap: 12px; padding: 20px; border-radius: 25px; font-weight: 800; font-size: 1rem; text-decoration: none; transition: 0.4s; margin-top: 15px; border: none; width: 100%; cursor: pointer; }
        .btn-whatsapp { background: #25d366; color: white; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); }
        .btn-call { background: var(--text); color: white; box-shadow: 0 10px 20px rgba(0,0,0,0.1); }
        .btn-action:hover { transform: scale(1.03); filter: brightness(1.1); }

        /* Floating Navigation Bar */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 400px; background: rgba(255,255,255,0.85); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.06); }
        .nav-icon { color: #8e8e93; font-size: 1.4rem; transition: 0.3s; }
        .nav-icon:hover { color: var(--primary); transform: scale(1.25); }

        footer { text-align: center; font-size: 0.75rem; opacity: 0.4; margin-top: 30px; line-height: 1.5; }
    </style>
</head>
<body>

    <div class="bg-canvas"></div>
    <div id="progress-bar"></div>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div style="background: rgba(79, 172, 254, 0.1); padding: 6px 15px; border-radius: 50px; display: inline-block; margin-bottom: 20px; font-size: 0.65rem; font-weight: 800; color: var(--primary); letter-spacing: 1px;">OFFICIAL PRIME SOLUTIONS PORTAL</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="font-size: 1.1rem; opacity: 0.7; font-weight: 300;">Founder & CEO | Prime Solutions</p>
            
            <div class="stats-row">
                <div class="stat-box"><h2>50+</h2><p>Projects</p></div>
                <div class="stat-box"><h2>15+</h2><p>Global Clients</p></div>
                <div class="stat-box"><h2>100%</h2><p>Trusted</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-code" style="color: var(--primary);"></i> Technical Expertise</h3>
            <div class="skill-box">
                <div class="skill-info"><span>Full-Stack Development</span><span>98%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 98%;"></div></div>
            </div>
            <div class="skill-box">
                <div class="skill-info"><span>UI/UX Architecture</span><span>95%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 95%;"></div></div>
            </div>
            <div class="skill-box">
                <div class="skill-info"><span>Firebase & Database</span><span>92%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 92%;"></div></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-gem" style="color: var(--primary);"></i> Unlimited Solutions</h3>
            <div class="badge-container">
                <div class="badge">E-commerce Stores</div>
                <div class="badge">Professional Portfolios</div>
                <div class="badge">Google SEO Mastery</div>
                <div class="badge">App Interface Design</div>
                <div class="badge">Real-time Chat Systems</div>
                <div class="badge">Investment Platforms</div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-stream"></i> Elite Strategy</h3>
            <div class="step">
                <div class="step-num">1</div>
                <div><h4 style="font-size: 0.9rem;">Analysis</h4><p style="font-size: 0.75rem; opacity: 0.6;">Aapke vision ko real business metrics mein convert karna.</p></div>
            </div>
            <div class="step">
                <div class="step-num">2</div>
                <div><h4 style="font-size: 0.9rem;">Modern Dev</h4><p style="font-size: 0.75rem; opacity: 0.6;">High-speed coding with zero-security risks.</p></div>
            </div>
            <div class="step">
                <div class="step-num">3</div>
                <div><h4 style="font-size: 0.9rem;">Deployment</h4><p style="font-size: 0.75rem; opacity: 0.6;">Final testing ke baad duniya ke liye live launch.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-left: 5px solid var(--primary);">
            <h3><i class="fas fa-shield-alt" style="color: var(--primary);"></i> Trusted Partnership</h3>
            <p style="font-size: 0.8rem; line-height: 1.6; opacity: 0.7; margin-top: 10px;">
                Prime Solutions 100% money-back guarantee aur professional NDA support ke sath kaam karta hai. Hamara har project lifelong maintenance ke sath aata hai.
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="background: linear-gradient(135deg, #ffffff, #f7fcff);">
            <h3 style="text-align: center; margin-bottom: 20px;">Start Your Journey</h3>
            <a href="https://wa.me/923332637235" class="btn-action btn-whatsapp" target="_blank">
                <i class="fab fa-whatsapp"></i> Chat on WhatsApp
            </a>
            <a href="tel:03705519562" class="btn-action btn-call">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
            <a href="mailto:webhub262@gmail.com" style="display: block; text-align: center; margin-top: 15px; font-size: 0.8rem; color: var(--primary); text-decoration: none; font-weight: 600;">
                <i class="fas fa-envelope-open"></i> webhub262@gmail.com
            </a>
        </div>

        <footer>
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Designed & Developed by Muhammad Nazim
        </footer>
    </div>

    <nav class="bottom-nav">
        <a href="#" class="nav-icon"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-icon"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-icon"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-icon"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Scroll Progress
        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
