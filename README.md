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
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        #progress-bar { position: fixed; top: 0; left: 0; width: 0%; height: 4px; background: linear-gradient(to right, var(--primary), var(--accent)); z-index: 9999; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay-mesh { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-image: radial-gradient(var(--primary) 0.5px, transparent 0.5px); background-size: 30px 30px; opacity: 0.1; z-index: -1; }

        .container { width: 100%; max-width: 480px; margin: 0 auto; padding: 60px 15px 120px; }

        /* Notification Bar */
        .top-notif { background: linear-gradient(to right, rgba(0,242,254,0.1), rgba(240,147,251,0.1)); padding: 8px; text-align: center; font-size: 0.6rem; border-bottom: 1px solid var(--border); letter-spacing: 1px; }

        .card { 
            background: var(--glass); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s;
        }

        /* Hero */
        .hero { text-align: center; }
        .profile-pic { width: 150px; height: 150px; border-radius: 50%; border: 2px solid var(--primary); padding: 6px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.3); }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; }

        /* Skill Bars */
        .skill-box { margin-bottom: 15px; }
        .skill-info { display: flex; justify-content: space-between; font-size: 0.8rem; margin-bottom: 5px; }
        .bar-bg { background: rgba(255,255,255,0.05); height: 8px; border-radius: 10px; }
        .bar-fill { height: 100%; border-radius: 10px; background: var(--primary); box-shadow: 0 0 10px var(--primary); }

        /* Timeline */
        .step { display: flex; gap: 15px; margin-bottom: 20px; }
        .step-num { min-width: 30px; height: 30px; border-radius: 50%; background: var(--primary); color: #000; display: flex; align-items: center; justify-content: center; font-weight: 800; font-size: 0.8rem; }

        /* Social Sidebar */
        .social-sidebar { position: fixed; right: 10px; top: 50%; transform: translateY(-50%); display: flex; flex-direction: column; gap: 15px; z-index: 100; }
        .social-sidebar i { font-size: 1.2rem; opacity: 0.5; transition: 0.3s; }
        .social-sidebar i:hover { opacity: 1; color: var(--primary); }

        .btn-premium { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; width: 100%; border-radius: 20px; font-weight: 800; border: none; font-size: 1rem; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; transition: 0.3s; }
        .btn-premium:hover { letter-spacing: 1px; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.3); }
    </style>
</head>
<body>

    <div id="progress-bar"></div>
    <div class="top-notif">🚀 PRIME SOLUTIONS IS NOW ACCEPTING GLOBAL PROJECTS 2026</div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay-mesh"></div>

    <div class="social-sidebar">
        <a href="https://wa.me/923332637235" style="color:white"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" style="color:white"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" style="color:white"><i class="fas fa-envelope"></i></a>
    </div>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p id="typewriter" style="font-size: 1.1rem; min-height: 25px; margin-top: 10px; color: var(--primary); font-weight: 300;"></p>
            <p style="font-size: 0.7rem; opacity: 0.5; margin-top: 10px;">Founder & Owner of Prime Solutions</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;">Agency Skills</h3>
            <div class="skill-box">
                <div class="skill-info"><span>Frontend Architecture</span><span>98%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 98%;"></div></div>
            </div>
            <div class="skill-box">
                <div class="skill-info"><span>Backend & Firebase</span><span>92%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 92%;"></div></div>
            </div>
            <div class="skill-box">
                <div class="skill-info"><span>UI/UX Modernism</span><span>95%</span></div>
                <div class="bar-bg"><div class="bar-fill" style="width: 95%;"></div></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 25px;">How We Work</h3>
            <div class="step">
                <div class="step-num">1</div>
                <div><h4>Consultation</h4><p style="font-size: 0.7rem; opacity: 0.6;">Aapke business goals par discussion.</p></div>
            </div>
            <div class="step">
                <div class="step-num">2</div>
                <div><h4>Strategy</h4><p style="font-size: 0.7rem; opacity: 0.6;">Design aur architecture ka plan.</p></div>
            </div>
            <div class="step">
                <div class="step-num">3</div>
                <div><h4>Development</h4><p style="font-size: 0.7rem; opacity: 0.6;">High-speed coding aur testing.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-top: 5px solid var(--primary);">
            <h3 style="text-align: center; margin-bottom: 20px;">Instant Inquiry</h3>
            <form id="infinityForm" style="display: flex; flex-direction: column; gap: 15px;">
                <input type="text" id="fname" placeholder="Full Name" required style="padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: rgba(255,255,255,0.02); color: white; outline: none;">
                <select id="fservice" required style="padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: #0a0a0a; color: white;">
                    <option value="" disabled selected>Service Selection</option>
                    <option value="Web Development">Full Web Development</option>
                    <option value="App Design">App Design</option>
                    <option value="Branding">Corporate Branding</option>
                </select>
                <textarea id="fmsg" placeholder="Project Details..." rows="2" style="padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: rgba(255,255,255,0.02); color: white; outline: none;"></textarea>
                <button type="submit" class="btn-premium"><i class="fab fa-whatsapp"></i> START PROJECT</button>
            </form>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.3; letter-spacing: 2px;">PRIME SOLUTIONS MASTERPIECE</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1200 });

        // Scroll Progress
        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        };

        // Typewriter
        const text = document.getElementById('typewriter');
        const phrases = ["Digital Architect", "Founder Prime Solutions", "Web Hub Owner", "UI/UX Visionary"];
        let i = 0, j = 0, isDeleting = false;
        function type() {
            const current = phrases[i];
            text.innerHTML = isDeleting ? current.substring(0, j--) : current.substring(0, j++);
            if (!isDeleting && j > current.length) { isDeleting = true; setTimeout(type, 2000); }
            else if (isDeleting && j < 0) { isDeleting = false; i = (i + 1) % phrases.length; setTimeout(type, 500); }
            else { setTimeout(type, isDeleting ? 50 : 100); }
        }
        window.onload = type;

        // WhatsApp Logic
        document.getElementById('infinityForm').addEventListener('submit', (e) => {
            e.preventDefault();
            const message = `*INQUIRY FROM PORTFOLIO*%0A*Name:* ${document.getElementById('fname').value}%0A*Service:* ${document.getElementById('fservice').value}%0A*Details:* ${document.getElementById('fmsg').value}`;
            window.open(`https://wa.me/923332637235?text=${message}`, '_blank');
        });
    </script>
</body>
</html>
