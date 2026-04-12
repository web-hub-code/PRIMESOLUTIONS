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
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        
        /* Custom Cursor */
        .cursor { width: 20px; height: 20px; border: 2px solid var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 9999; transition: transform 0.1s; transform: translate(-50%, -50%); box-shadow: 0 0 15px var(--primary); }

        .container { width: 100%; max-width: 480px; margin: 0 auto; padding: 20px 15px 150px; }

        /* Fake Live Notification */
        .notification { position: fixed; bottom: 120px; left: 20px; background: rgba(255,255,255,0.1); backdrop-filter: blur(15px); padding: 10px 20px; border-radius: 20px; border: 1px solid var(--primary); font-size: 0.7rem; display: flex; align-items: center; gap: 10px; z-index: 1000; transform: translateX(-150%); transition: 0.5s; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }
        .notification.active { transform: translateX(0); }

        /* Premium Hero */
        .card { 
            background: var(--glass); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 40px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s;
        }
        .hero { text-align: center; }
        .profile-pic { width: 150px; height: 150px; border-radius: 50%; border: 2px solid var(--primary); padding: 6px; box-shadow: 0 0 40px rgba(0, 242, 254, 0.3); }
        
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; }

        /* Trust Badges */
        .trust-icons { display: flex; justify-content: center; gap: 20px; margin-top: 20px; opacity: 0.5; font-size: 1.2rem; }

        /* Floating WA */
        .wa-float { position: fixed; bottom: 30px; right: 20px; background: #25d366; color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 32px; z-index: 1001; animation: pulse 2s infinite; text-decoration: none; cursor: pointer; }
        @keyframes pulse { 0% { transform: scale(1); box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7); } 70% { transform: scale(1.05); box-shadow: 0 0 0 15px rgba(37, 211, 102, 0); } 100% { transform: scale(1); } }

        /* Nav Bar */
        .nav-bar { position: fixed; bottom: 30px; left: 20px; width: calc(100% - 110px); max-width: 320px; background: rgba(255,255,255,0.05); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; transition: 0.3s; cursor: pointer; }
        .nav-link:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        .btn-hire { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; border: none; font-size: 1.1rem; cursor: pointer; margin-top: 20px; }
    </style>
</head>
<body>

    <div class="cursor" id="cursor"></div>
    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <div class="notification" id="notif">
        <i class="fas fa-shopping-cart" style="color: var(--primary);"></i>
        <span id="notif-text">New project started in Lahore!</span>
    </div>

    <a href="https://wa.me/923332637235" class="wa-float" target="_blank"><i class="fab fa-whatsapp"></i></a>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div style="background: rgba(0,242,254,0.1); color: var(--primary); display: inline-block; padding: 5px 15px; border-radius: 50px; font-size: 0.6rem; font-weight: 800; margin-bottom: 15px;">TOP RATED AGENCY 2026</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p id="typewriter" style="font-size: 1.1rem; color: var(--primary); font-weight: 300;"></p>
            
            <div class="trust-icons">
                <i class="fab fa-google"></i> <i class="fab fa-stripe"></i> <i class="fas fa-shield-alt"></i> <i class="fab fa-amazon"></i>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;">Elite Solutions</h3>
            <div style="display: grid; gap: 15px;">
                <div style="background: rgba(255,255,255,0.02); padding: 15px; border-radius: 20px; border: 1px solid var(--border);">
                    <i class="fas fa-check-circle" style="color: var(--primary);"></i> <b>Premium Branding:</b> Apple-style modern aesthetics.
                </div>
                <div style="background: rgba(255,255,255,0.02); padding: 15px; border-radius: 20px; border: 1px solid var(--border);">
                    <i class="fas fa-check-circle" style="color: var(--primary);"></i> <b>Fast Delivery:</b> Projects ready within 48-72 hours.
                </div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 5px solid var(--primary);">
            <h3 style="text-align: center;"><i class="fas fa-user-lock"></i> 100% Trusted</h3>
            <p style="text-align: center; font-size: 0.8rem; opacity: 0.6; margin-top: 10px;">End-to-end encryption for all client data. Money-back guarantee if not satisfied.</p>
            <a href="https://wa.me/923332637235" class="btn-hire">START YOUR PROJECT</a>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.2;">PRIME SOLUTIONS | EXCELLENCE IN CODE</footer>
    </div>

    <nav class="nav-bar">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000 });

        // Cursor Movement
        const cursor = document.getElementById('cursor');
        document.addEventListener('mousemove', e => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
        });

        // Typewriter
        const text = document.getElementById('typewriter');
        const phrases = ["Founder Prime Solutions", "Digital Architect", "UI/UX Specialist"];
        let i = 0, j = 0;
        function type() {
            if (j < phrases[i].length) { text.innerHTML += phrases[i][j]; j++; setTimeout(type, 100); }
            else { setTimeout(erase, 2000); }
        }
        function erase() {
            if (j > 0) { text.innerHTML = phrases[i].substring(0, j-1); j--; setTimeout(erase, 50); }
            else { i = (i + 1) % phrases.length; setTimeout(type, 500); }
        }
        window.onload = type;

        // Social Proof Notification Logic
        const notif = document.getElementById('notif');
        const notifText = document.getElementById('notif-text');
        const cities = ["Karachi", "Lahore", "Dubai", "London", "New York"];
        function showNotif() {
            const city = cities[Math.floor(Math.random() * cities.length)];
            notifText.innerText = `New order from ${city}!`;
            notif.classList.add('active');
            setTimeout(() => notif.classList.remove('active'), 4000);
        }
        setInterval(showNotif, 10000);
    </script>
</body>
</html>
