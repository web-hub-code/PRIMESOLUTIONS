<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | CEO Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
            --card-bg: rgba(255, 255, 255, 0.04);
        }
        
        .light-theme {
            --bg: #f0f2f5; --glass: rgba(255, 255, 255, 0.8); --border: rgba(0, 0, 0, 0.1);
            --card-bg: #ffffff; color: #1a1a1a;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; transition: background 0.3s, color 0.3s; }
        body { background-color: var(--bg); overflow-x: hidden; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .light-theme #bg-video { display: none; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        .card { 
            background: var(--glass); backdrop-filter: blur(25px); 
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 28px; margin-bottom: 22px; transition: 0.5s;
        }
        
        /* Theme Toggle */
        .theme-btn { position: fixed; top: 20px; right: 20px; z-index: 1002; background: var(--primary); color: #000; border: none; width: 45px; height: 45px; border-radius: 15px; cursor: pointer; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; box-shadow: 0 5px 15px rgba(0, 242, 254, 0.3); }

        /* Pricing Cards */
        .price-card { background: rgba(255,255,255,0.03); border: 1px solid var(--border); border-radius: 25px; padding: 20px; margin-top: 15px; text-align: center; }
        .price-tag { font-size: 1.5rem; font-weight: 800; color: var(--primary); margin: 10px 0; }
        
        /* Floating Elements */
        .wa-float { position: fixed; bottom: 100px; right: 20px; background: #25d366; color: white; width: 55px; height: 55px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 30px; z-index: 1001; animation: pulse 2s infinite; text-decoration: none; }
        @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.1); } 100% { transform: scale(1); } }

        .hero { text-align: center; padding: 40px 10px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.4); object-fit: cover; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10, 10, 10, 0.9); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; }
        
        .btn-primary { background: linear-gradient(45deg, #00f2fe, #4facfe); color: #000; padding: 15px; width: 100%; border-radius: 20px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 10px; border: none; cursor: pointer; }
    </style>
</head>
<body id="body">

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <button class="theme-btn" onclick="toggleTheme()"><i class="fas fa-moon" id="theme-icon"></i></button>
    <a href="https://wa.me/923332637235" class="wa-float" target="_blank"><i class="fab fa-whatsapp"></i></a>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <div id="typewriter" style="color: var(--primary); height: 20px;"></div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-tags" style="color: var(--primary);"></i> Service Packages</h3>
            <div class="price-card">
                <h4>Starter Pack</h4>
                <p class="price-tag">Starting 250 PKR</p>
                <p style="font-size: 0.7rem; opacity: 0.7;">Single Landing Page • SEO Ready</p>
                <button class="btn-primary" onclick="location.href='https://wa.me/923332637235'">Select Starter</button>
            </div>
            <div class="price-card" style="border-color: var(--accent);">
                <h4 style="color: var(--accent);">Pro Agency</h4>
                <p class="price-tag">Custom Quote</p>
                <p style="font-size: 0.7rem; opacity: 0.7;">Full Dashboard • Firebase • UI/UX</p>
                <button class="btn-primary" style="background: var(--accent);" onclick="location.href='https://wa.me/923332637235'">Go Pro</button>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-paper-plane"></i> Stay Updated</h3>
            <div style="margin-top: 15px; display: flex; gap: 10px;">
                <input type="email" placeholder="Your Email" style="flex: 1; padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: rgba(255,255,255,0.05); color: white;">
                <button style="padding: 15px; border-radius: 15px; background: var(--primary); border: none; cursor: pointer;"><i class="fas fa-check"></i></button>
            </div>
        </div>

        <nav class="nav-bar">
            <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
            <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
            <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
            <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
        </nav>
        
        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.4;">© 2026 PRIME SOLUTIONS | CEO NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000 });

        function toggleTheme() {
            const body = document.getElementById('body');
            const icon = document.getElementById('theme-icon');
            body.classList.toggle('light-theme');
            icon.classList.toggle('fa-moon');
            icon.classList.toggle('fa-sun');
        }

        const text = document.getElementById('typewriter');
        const phrases = ["Founder Prime Solutions", "Digital Architect", "Firebase Specialist"];
        let i = 0; let j = 0;
        function type() {
            if (j < phrases[i].length) { text.innerHTML += phrases[i][j]; j++; setTimeout(type, 100); }
            else { setTimeout(erase, 2000); }
        }
        function erase() {
            if (j > 0) { text.innerHTML = phrases[i].substring(0, j-1); j--; setTimeout(erase, 50); }
            else { i = (i + 1) % phrases.length; setTimeout(type, 500); }
        }
        window.onload = type;
    </script>
</body>
</html>
