<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Master</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #fdfdfd; --text: #1d1d1f; --card: rgba(255, 255, 255, 0.9); --border: rgba(0, 0, 0, 0.08);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Floating Modern Nav */
        .glass-nav { position: sticky; top: 15px; z-index: 1000; background: var(--card); backdrop-filter: blur(15px); border-radius: 25px; padding: 15px; border: 1px solid var(--border); display: flex; justify-content: space-between; align-items: center; margin-bottom: 30px; }

        /* Hero Glitch Effect */
        .hero-title { font-size: 2.2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; }

        .card { 
            background: var(--card); backdrop-filter: blur(20px); border: 1px solid var(--border); 
            border-radius: 30px; padding: 25px; margin-bottom: 25px; box-shadow: 0 10px 30px rgba(0,0,0,0.03);
        }

        /* Animated Stats */
        .stat-box { text-align: center; padding: 15px; background: rgba(79, 172, 254, 0.1); border-radius: 20px; }
        .stat-number { font-size: 1.8rem; font-weight: 800; color: var(--primary); }

        /* Timeline Feature */
        .timeline { border-left: 2px dashed var(--primary); margin: 20px 0 20px 20px; padding-left: 20px; }
        .timeline-item { position: relative; margin-bottom: 25px; }
        .timeline-item::before { content: ''; position: absolute; left: -31px; top: 5px; width: 20px; height: 20px; background: var(--primary); border-radius: 50%; box-shadow: 0 0 10px var(--primary); }

        /* Glowing Quote Form */
        .premium-input { width: 100%; padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: rgba(0,0,0,0.02); color: var(--text); margin-bottom: 15px; }
        .btn-glow { width: 100%; padding: 18px; border-radius: 20px; border: none; background: linear-gradient(45deg, var(--primary), var(--secondary)); color: white; font-weight: 800; cursor: pointer; box-shadow: 0 10px 20px rgba(79, 172, 254, 0.3); }

        .service-tag { display: inline-block; padding: 8px 15px; background: rgba(79, 172, 254, 0.1); border-radius: 50px; font-size: 0.7rem; margin: 5px; font-weight: 600; color: var(--primary); }
    </style>
</head>
<body data-theme="light">

    <div class="container">
        
        <nav class="glass-nav">
            <span style="font-weight: 800; color: var(--primary);">PRIME SOLUTIONS</span>
            <div onclick="toggleTheme()" style="cursor: pointer;"><i class="fas fa-adjust"></i></div>
        </nav>

        <section class="card" data-aos="zoom-in">
            <div style="text-align: center;">
                <div style="background: #25d366; color: white; padding: 5px 15px; border-radius: 50px; font-size: 0.6rem; display: inline-block; margin-bottom: 10px; font-weight: 800;">ACTIVE NOW</div>
                <h1 class="hero-title">Muhammad Nazim</h1>
                <p style="opacity: 0.6; font-size: 0.85rem; margin-top: 5px;">Creative Web Developer & Agency Owner</p>
            </div>
            
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 25px;">
                <div class="stat-box"><div class="stat-number">150+</div><p style="font-size: 0.6rem;">PROJECTS</p></div>
                <div class="stat-box"><div class="stat-number">99%</div><p style="font-size: 0.6rem;">SUCCESS</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-stream"></i> Our Working Process</h3>
            <div class="timeline">
                <div class="timeline-item"><h4>Discussion</h4><p style="font-size: 0.7rem; opacity: 0.6;">Understanding your business needs.</p></div>
                <div class="timeline-item"><h4>Design UI</h4><p style="font-size: 0.7rem; opacity: 0.6;">Creating a mobile-first attractive look.</p></div>
                <div class="timeline-item"><h4>Development</h4><p style="font-size: 0.7rem; opacity: 0.6;">Coding with high security & speed.</p></div>
                <div class="timeline-item"><h4>Launch</h4><p style="font-size: 0.7rem; opacity: 0.6;">Live on your custom domain.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-laptop-code"></i> Industry Solutions</h3>
            <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 15px;">We build for every business type</p>
            <div style="display: flex; wrap: wrap;">
                <span class="service-tag">Real Estate</span>
                <span class="service-tag">E-Commerce</span>
                <span class="service-tag">Crypto/Forex</span>
                <span class="service-tag">Educational</span>
                <span class="service-tag">Personal Portfolio</span>
                <span class="service-tag">Investment</span>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-file-invoice-dollar"></i> Request a Project</h3>
            <div style="margin-top: 15px;">
                <input type="text" id="clientName" class="premium-input" placeholder="Your Full Name">
                <select id="serviceType" class="premium-input">
                    <option>Standard Business Site</option>
                    <option>Investment Platform (Pakgold Style)</option>
                    <option>E-commerce Web App</option>
                    <option>UI/UX Design Only</option>
                </select>
                <textarea id="projectDetails" class="premium-input" rows="3" placeholder="Briefly describe your project idea..."></textarea>
                <button class="btn-glow" onclick="submitRequest()"><i class="fab fa-whatsapp"></i> SUBMIT TO WHATSAPP</button>
            </div>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.4; margin-top: 20px;">
            VERIFIED PRIME SOLUTIONS PORTAL 2026<br>
            SECURE | TRUSTED | FAST
        </footer>

    </div>

    <div style="position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; background: var(--card); backdrop-filter: blur(15px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 2000; box-shadow: 0 15px 30px rgba(0,0,0,0.1);">
        <a href="tel:03705519562" style="color: var(--text);"><i class="fas fa-phone-alt"></i></a>
        <a href="https://wa.me/923332637235" style="color: #25d366; font-size: 1.5rem;"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" style="color: #1877F2;"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" style="color: #ea4335;"><i class="fas fa-envelope"></i></a>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function toggleTheme() {
            const body = document.body;
            body.setAttribute('data-theme', body.getAttribute('data-theme') === 'light' ? 'dark' : 'light');
        }

        function submitRequest() {
            const name = document.getElementById('clientName').value;
            const type = document.getElementById('serviceType').value;
            const detail = document.getElementById('projectDetails').value;
            const text = `Hello Nazim! I am ${name}. I need a ${type}. Project Detail: ${detail}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
