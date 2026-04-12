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
            --bg: #fdfdfd; --text: #1d1d1f; --card-bg: rgba(255, 255, 255, 0.8); --border: rgba(0, 0, 0, 0.08);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card-bg: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; transition: background 0.3s, color 0.3s; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Theme Toggle Button */
        .theme-switch { position: fixed; top: 20px; right: 20px; z-index: 2000; background: var(--card-bg); border: 1px solid var(--border); padding: 12px; border-radius: 50%; cursor: pointer; backdrop-filter: blur(10px); color: var(--primary); box-shadow: 0 5px 15px rgba(0,0,0,0.05); }

        #progress-bar { position: fixed; top: 0; left: 0; width: 0%; height: 4px; background: linear-gradient(to right, var(--primary), var(--accent)); z-index: 9999; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 60px 15px 120px; }

        /* Unlimited Extra Feature: Glass Cards */
        .card { 
            background: var(--card-bg); backdrop-filter: blur(25px); -webkit-backdrop-filter: blur(25px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 40px rgba(0,0,0,0.04); cursor: pointer;
        }
        .card:hover { transform: translateY(-10px) scale(1.02); border-color: var(--primary); box-shadow: 0 25px 50px rgba(79, 172, 254, 0.15); }

        /* Extra Details: Interactive Badges */
        .badge-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 15px; }
        .mini-badge { background: rgba(79, 172, 254, 0.1); padding: 10px; border-radius: 15px; font-size: 0.7rem; font-weight: 600; display: flex; align-items: center; gap: 8px; color: var(--primary); }

        /* Professional Stats */
        .stat-line { display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px; font-size: 0.8rem; }
        .stat-bar { height: 6px; background: rgba(0,0,0,0.05); border-radius: 10px; overflow: hidden; margin-bottom: 15px; }
        .stat-fill { height: 100%; background: linear-gradient(90deg, var(--primary), var(--secondary)); }

        /* Trusted Features: Testimonials & Security */
        .trust-box { border-left: 4px solid #25d366; background: rgba(37, 211, 102, 0.05); padding: 15px; border-radius: 0 20px 20px 0; margin-top: 15px; font-size: 0.8rem; }

        /* Floating Nav */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 400px; background: var(--card-bg); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .nav-icon { color: var(--text); opacity: 0.6; font-size: 1.4rem; transition: 0.3s; text-decoration: none; }
        .nav-icon:hover { color: var(--primary); opacity: 1; transform: translateY(-5px); }

        .btn-main { display: flex; align-items: center; justify-content: center; gap: 12px; padding: 20px; border-radius: 25px; font-weight: 800; text-decoration: none; margin-top: 15px; color: white; transition: 0.4s; }
        .btn-wa { background: #25d366; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); }
    </style>
</head>
<body data-theme="light">

    <div class="theme-switch" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>
    <div id="progress-bar"></div>

    <div class="container">
        <section class="card" data-aos="zoom-in" style="text-align: center;">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" style="width: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px;">
            <h1 style="font-size: 2.2rem; font-weight: 800; background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
            <p style="opacity: 0.7; font-size: 0.9rem;">Founder | Prime Solutions Official</p>
            
            <div class="badge-grid">
                <div class="mini-badge"><i class="fas fa-check-circle"></i> Verified Dev</div>
                <div class="mini-badge"><i class="fas fa-shield-alt"></i> Secure Code</div>
                <div class="mini-badge"><i class="fas fa-clock"></i> 24/7 Active</div>
                <div class="mini-badge"><i class="fas fa-star"></i> Top Rated</div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-chart-line" style="color: var(--primary);"></i> Mastery & Accuracy</h3>
            <div class="stat-line"><span>Web Architecture</span><span>98%</span></div>
            <div class="stat-bar"><div class="stat-fill" style="width: 98%;"></div></div>
            <div class="stat-line"><span>Firebase / Database</span><span>95%</span></div>
            <div class="stat-bar"><div class="stat-fill" style="width: 95%;"></div></div>
            <div class="stat-line"><span>SEO Ranking</span><span>90%</span></div>
            <div class="stat-bar"><div class="stat-fill" style="width: 90%;"></div></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-heart" style="color: var(--accent);"></i> Trusted by Millions</h3>
            <div class="trust-box">
                "Nazim built our business site (Web-Hub) in record time. Professionalism at its peak!"
            </div>
            <div class="trust-box" style="border-left-color: var(--primary);">
                "Pakgold platform deployment was seamless. Highly recommended for investment sites."
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-th-large"></i> Elite Services</h3>
            <p style="font-size: 0.8rem; opacity: 0.6; margin-bottom: 15px;">(Click to inquire via WhatsApp)</p>
            <div style="display: flex; flex-direction: column; gap: 10px;">
                <a href="https://wa.me/923332637235?text=I'm interested in Web Development" class="mini-badge" style="text-decoration: none; cursor: pointer;"><i class="fas fa-code"></i> Full-Stack Web Dev</a>
                <a href="https://wa.me/923332637235?text=I'm interested in UI/UX Design" class="mini-badge" style="text-decoration: none; cursor: pointer;"><i class="fas fa-paint-brush"></i> Premium UI/UX Design</a>
                <a href="https://wa.me/923332637235?text=I'm interested in SEO Services" class="mini-badge" style="text-decoration: none; cursor: pointer;"><i class="fas fa-search"></i> Advanced SEO Ranking</a>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="background: linear-gradient(135deg, var(--card-bg), rgba(79, 172, 254, 0.05));">
            <h3 style="text-align: center;">Let's Talk Business</h3>
            <p style="text-align: center; font-size: 0.8rem; opacity: 0.7; margin-top: 10px;">Secure your digital future with Prime Solutions.</p>
            
            <a href="https://wa.me/923332637235" class="btn-main btn-wa" target="_blank">
                <i class="fab fa-whatsapp"></i> Get Free Consultation
            </a>
            
            <a href="tel:03705519562" class="btn-main" style="background: var(--text); color: var(--bg); border: 1px solid var(--border);">
                <i class="fas fa-phone-alt"></i> Direct Call: 0370 5519562
            </a>

            <p style="text-align: center; font-size: 0.7rem; margin-top: 15px; opacity: 0.5;">
                <i class="fas fa-envelope"></i> webhub262@gmail.com
            </p>
        </div>

        <footer style="text-align: center; font-size: 0.75rem; opacity: 0.4;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Powered by Nazim's Innovation
        </footer>
    </div>

    <nav class="bottom-nav">
        <a href="#" class="nav-icon"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-icon"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-icon"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-icon"><i class="fas fa-envelope-open"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function toggleTheme() {
            const body = document.body;
            const icon = document.querySelector('.theme-switch i');
            if(body.getAttribute('data-theme') === 'light') {
                body.setAttribute('data-theme', 'dark');
                icon.className = 'fas fa-sun';
            } else {
                body.setAttribute('data-theme', 'light');
                icon.className = 'fas fa-moon';
            }
        }

        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
