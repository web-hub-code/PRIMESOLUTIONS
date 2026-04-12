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
            --glow: rgba(79, 172, 254, 0.2);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
            --glow: rgba(255, 255, 255, 0.05);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: 0.4s ease; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Scroll Tracker */
        #scroll-tracker { position: fixed; top: 0; left: 0; width: 0%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); z-index: 9999; }

        /* Premium Slider */
        .swiper { width: 100%; height: 260px; border-radius: 0 0 45px 45px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
        .swiper-slide img { width: 100%; height: 100%; object-fit: cover; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 30px 15px 120px; }

        .card { 
            background: var(--card); backdrop-filter: blur(30px); border: 1px solid var(--border); 
            border-radius: 35px; padding: 25px; margin-bottom: 25px; position: relative;
            box-shadow: 0 15px 35px rgba(0,0,0,0.03);
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 20px 45px var(--glow); }

        /* Header Controls */
        .header-tools { position: fixed; top: 20px; right: 20px; z-index: 3000; display: flex; gap: 10px; }
        .tool-btn { background: var(--card); border: 1px solid var(--border); padding: 12px; border-radius: 50%; cursor: pointer; backdrop-filter: blur(15px); color: var(--primary); box-shadow: 0 8px 15px rgba(0,0,0,0.1); }

        /* Form Styling */
        .input-box { width: 100%; padding: 15px; border-radius: 18px; border: 1px solid var(--border); background: rgba(0,0,0,0.02); color: var(--text); margin-bottom: 15px; outline: none; }
        .btn-submit { width: 100%; padding: 20px; border-radius: 25px; border: none; background: linear-gradient(45deg, var(--primary), var(--secondary)); color: white; font-weight: 800; cursor: pointer; box-shadow: 0 12px 24px rgba(79, 172, 254, 0.3); font-size: 1rem; }

        /* Process Timeline */
        .process-flow { border-left: 2px dashed var(--primary); margin: 20px 0 20px 20px; padding-left: 25px; }
        .step { position: relative; margin-bottom: 30px; }
        .step::before { content: ''; position: absolute; left: -36px; top: 5px; width: 20px; height: 20px; background: var(--primary); border-radius: 50%; border: 4px solid var(--bg); }

        /* Bottom Menu */
        .nav-hub { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 420px; background: var(--card); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .nav-item { color: var(--text); opacity: 0.5; font-size: 1.4rem; text-decoration: none; }
        .nav-item.active { color: var(--primary); opacity: 1; transform: translateY(-3px); }

        .service-pill { display: inline-block; padding: 8px 16px; background: rgba(79, 172, 254, 0.1); border-radius: 50px; font-size: 0.75rem; margin: 5px; font-weight: 600; color: var(--primary); border: 1px solid rgba(79, 172, 254, 0.1); }
    </style>
</head>
<body data-theme="light">

    <div id="scroll-tracker"></div>

    <div class="header-tools">
        <div class="tool-btn" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>
    </div>

    <div class="swiper mySwiper">
        <div class="swiper-wrapper">
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=2426&auto=format&fit=crop"></div>
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=2344&auto=format&fit=crop"></div>
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?q=80&w=2340&auto=format&fit=crop"></div>
        </div>
        <div class="swiper-pagination"></div>
    </div>

    <div class="container">
        
        <section class="card" data-aos="zoom-in" style="text-align: center;">
            <div style="background: rgba(37, 211, 102, 0.1); color: #25d366; padding: 6px 15px; border-radius: 50px; font-size: 0.65rem; display: inline-block; margin-bottom: 12px; font-weight: 800; border: 1px solid rgba(37, 211, 102, 0.2);">
                <i class="fas fa-shield-check"></i> VERIFIED MASTER DEVELOPER
            </div>
            <h1 style="font-size: 2.5rem; font-weight: 800; background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
            <p style="opacity: 0.6; font-size: 0.9rem; margin-top: 5px;">CEO & Founder | Prime Solutions Agency</p>
            
            <div style="display: flex; justify-content: center; gap: 20px; margin-top: 25px;">
                <div style="text-align: center;"><h3>150+</h3><p style="font-size: 0.6rem; opacity: 0.5;">PROJECTS</p></div>
                <div style="width: 1px; height: 30px; background: var(--border);"></div>
                <div style="text-align: center;"><h3>100%</h3><p style="font-size: 0.6rem; opacity: 0.5;">SATISFACTION</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-project-diagram" style="color: var(--primary);"></i> Development Roadmap</h3>
            <div class="process-flow">
                <div class="step"><h4>Consultation</h4><p style="font-size: 0.75rem; opacity: 0.6;">Discussing goals and target audience.</p></div>
                <div class="step"><h4>Strategic UI</h4><p style="font-size: 0.75rem; opacity: 0.6;">Designing interactive & fast interfaces.</p></div>
                <div class="step"><h4>Master Coding</h4><p style="font-size: 0.75rem; opacity: 0.6;">High-level programming with security.</p></div>
                <div class="step"><h4>Global Launch</h4><p style="font-size: 0.75rem; opacity: 0.6;">Deploying on GitHub/Netlify/Custom VPS.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-boxes-stacked"></i> Business Solutions</h3>
            <div style="margin-top: 15px;">
                <span class="service-pill">E-Commerce Ecosystems</span>
                <span class="service-pill">Investment Dashboards</span>
                <span class="service-pill">Real Estate Portals</span>
                <span class="service-pill">Financial CMS</span>
                <span class="service-pill">School Management</span>
                <span class="service-pill">Custom Web Apps</span>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-file-invoice"></i> Get a Free Estimate</h3>
            <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 20px;">We respond within 30 minutes.</p>
            
            <input type="text" id="name" class="input-box" placeholder="Your Name">
            <select id="ptype" class="input-box">
                <option>Investment Platform (Pakgold Style)</option>
                <option>Business/Portfolio Site</option>
                <option>Multi-Vendor E-commerce</option>
                <option>Educational App</option>
            </select>
            <select id="delivery" class="input-box">
                <option value="whatsapp">Send via WhatsApp</option>
                <option value="email">Send via Email</option>
            </select>
            <textarea id="desc" class="input-box" rows="3" placeholder="Tell us about your project..."></textarea>
            
            <button class="btn-submit" onclick="submitInquiry()">LAUNCH INQUIRY NOW</button>
        </div>

        <footer style="text-align: center; font-size: 0.75rem; opacity: 0.4;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Coded with Excellence by Nazim
        </footer>
    </div>

    <nav class="nav-hub">
        <a href="tel:03705519562" class="nav-item"><i class="fas fa-phone-volume"></i></a>
        <a href="https://wa.me/923332637235" class="nav-item" style="color: #25d366; font-size: 1.8rem;"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope-open-text"></i></a>
    </nav>

    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        var swiper = new Swiper(".mySwiper", {
            pagination: { el: ".swiper-pagination", dynamicBullets: true },
            autoplay: { delay: 3500 },
            loop: true,
            effect: "fade"
        });

        function toggleTheme() {
            const body = document.body;
            const icon = document.querySelector('.tool-btn i');
            const isDark = body.getAttribute('data-theme') === 'dark';
            body.setAttribute('data-theme', isDark ? 'light' : 'dark');
            icon.className = isDark ? 'fas fa-moon' : 'fas fa-sun';
        }

        function submitInquiry() {
            const name = document.getElementById('name').value;
            const type = document.getElementById('ptype').value;
            const delivery = document.getElementById('delivery').value;
            const desc = document.getElementById('desc').value;
            const text = `Hello Nazim! My name is ${name}. I am looking for a ${type}. Details: ${desc}`;
            
            if(delivery === 'whatsapp') {
                window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
            } else {
                window.location.href = `mailto:webhub262@gmail.com?subject=New Agency Inquiry&body=${encodeURIComponent(text)}`;
            }
        }

        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("scroll-tracker").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
