<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sulza Design | Web Development & Data Analysis</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://site-assets.fontawesome.com/releases/v6.5.0/css/all.css">
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&family=Inter:wght@400;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #1e293b; /* Deep Navy */
            --accent: #D4AF37;  /* Gold */
            --bg-light: #f8fafc;
        }
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: var(--bg-light); 
            color: var(--primary);
        }
        .text-accent { color: var(--accent); }
        .bg-accent { background-color: var(--accent); }
        
        /* Smooth shadows for a professional look */
        .soft-shadow { box-shadow: 0 10px 30px -10px rgba(0,0,0,0.08); }
        .card:hover { transform: translateY(-5px); box-shadow: 0 20px 40px -15px rgba(0,0,0,0.12); }
        
        .nav-blur {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid #e2e8f0;
        }

        /* Image hover effect */
        .img-zoom { overflow: hidden; }
        .img-zoom img { transition: transform 0.5s ease; }
        .img-zoom:hover img { transform: scale(1.05); }
    </style>
</head>
<body>

    <nav class="fixed w-full z-50 py-4 px-6 md:px-12 flex justify-between items-center nav-blur">
        <div class="flex items-center gap-3">
            <div class="w-10 h-10 bg-primary text-white flex items-center justify-center rounded-xl font-bold text-xl" style="background: #1e293b;">S</div>
            <div class="text-xl font-extrabold tracking-tighter text-slate-900">SULZA<span class="text-accent">DESIGN</span></div>
        </div>
        <div class="hidden md:flex gap-8 text-[12px] font-bold uppercase tracking-widest text-slate-600">
            <a href="#services" class="hover:text-accent transition">Services</a>
            <a href="#work" class="hover:text-accent transition">Portfolio</a>
            <a href="#about" class="hover:text-accent transition">About</a>
            <a href="#contact" class="hover:text-accent transition">Contact</a>
        </div>
        <a href="https://wa.me/2348149247947" class="bg-slate-900 text-white px-6 py-2.5 rounded-lg font-bold text-xs uppercase hover:bg-accent transition">Hire Us</a>
    </nav>

    <section class="min-h-screen pt-32 pb-20 px-6 flex flex-col items-center justify-center text-center bg-white">
        <div class="max-w-4xl">
            <span class="inline-block py-1.5 px-4 rounded-full bg-slate-100 text-slate-600 text-[11px] font-bold uppercase tracking-[0.2em] mb-6">Innovative IT Solutions</span>
            <h1 class="text-5xl md:text-7xl font-extrabold text-slate-900 leading-[1.1] mb-8">
                Turning Complex Logic into <span class="text-accent">Beautiful Systems.</span>
            </h1>
            <p class="text-slate-500 text-lg md:text-xl max-w-2xl mx-auto mb-12 leading-relaxed">
                Expert Web Development, Data Science, and Strategic Design tailored for growth-oriented businesses.
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#work" class="bg-slate-900 text-white px-10 py-4 rounded-xl font-bold soft-shadow hover:scale-105 transition">View Case Studies</a>
                <a href="#contact" class="bg-white border border-slate-200 px-10 py-4 rounded-xl font-bold hover:bg-slate-50 transition">Start a Project</a>
            </div>
        </div>
    </section>

    <section id="services" class="py-24 px-6 md:px-20">
        <div class="max-w-7xl mx-auto grid md:grid-cols-4 gap-8">
            <div class="bg-white p-8 rounded-3xl soft-shadow card transition-all border border-slate-50">
                <div class="w-14 h-14 bg-blue-50 text-blue-600 rounded-2xl flex items-center justify-center mb-6 text-2xl">
                    <i class="fa-light fa-code"></i>
                </div>
                <h3 class="text-xl font-bold mb-3 text-slate-900">Web Development</h3>
                <p class="text-slate-500 text-sm leading-relaxed">Scalable full-stack apps using PHP, MySQL, and modern JS frameworks.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl soft-shadow card transition-all border border-slate-50">
                <div class="w-14 h-14 bg-amber-50 text-amber-600 rounded-2xl flex items-center justify-center mb-6 text-2xl">
                    <i class="fa-light fa-chart-mixed"></i>
                </div>
                <h3 class="text-xl font-bold mb-3 text-slate-900">Data Analysis</h3>
                <p class="text-slate-500 text-sm leading-relaxed">Transforming data into interactive dashboards and actionable intelligence.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl soft-shadow card transition-all border border-slate-50">
                <div class="w-14 h-14 bg-purple-50 text-purple-600 rounded-2xl flex items-center justify-center mb-6 text-2xl">
                    <i class="fa-light fa-bezier-curve"></i>
                </div>
                <h3 class="text-xl font-bold mb-3 text-slate-900">Graphics Design</h3>
                <p class="text-slate-500 text-sm leading-relaxed">Premium branding, social media content, and high-fidelity UI/UX design.</p>
            </div>
            <div class="bg-white p-8 rounded-3xl soft-shadow card transition-all border border-slate-50">
                <div class="w-14 h-14 bg-emerald-50 text-emerald-600 rounded-2xl flex items-center justify-center mb-6 text-2xl">
                    <i class="fa-light fa-shield-check"></i>
                </div>
                <h3 class="text-xl font-bold mb-3 text-slate-900">IT Consulting</h3>
                <p class="text-slate-500 text-sm leading-relaxed">Cybersecurity auditing, network optimization, and tech strategy.</p>
            </div>
        </div>
    </section>

    <section id="work" class="py-24 px-6 md:px-20 bg-slate-50">
        <div class="max-w-7xl mx-auto">
            <div class="mb-16">
                <h2 class="text-4xl font-extrabold text-slate-900 mb-4">Featured Work</h2>
                <div class="w-20 h-1.5 bg-accent rounded-full"></div>
            </div>

            <div class="grid md:grid-cols-2 gap-10">
                <div class="group">
                    <div class="img-zoom rounded-3xl soft-shadow mb-6 aspect-video bg-slate-200">
                        <img src="https://via.placeholder.com/800x450" alt="Project 1" class="w-full h-full object-cover">
                    </div>
                    <div class="px-2">
                        <span class="text-accent text-xs font-bold uppercase tracking-widest">Web Application</span>
                        <h4 class="text-2xl font-bold text-slate-900 mt-2">StudyAI Learning Management</h4>
                        <p class="text-slate-500 mt-3 text-sm">Full-stack development of a personalized AI-driven education platform.</p>
                    </div>
                </div>
                <div class="group">
                    <div class="img-zoom rounded-3xl soft-shadow mb-6 aspect-video bg-slate-200">
                        <img src="https://via.placeholder.com/800x450" alt="Project 2" class="w-full h-full object-cover">
                    </div>
                    <div class="px-2">
                        <span class="text-accent text-xs font-bold uppercase tracking-widest">Branding & Design</span>
                        <h4 class="text-2xl font-bold text-slate-900 mt-2">Corporate Identity Package</h4>
                        <p class="text-slate-500 mt-3 text-sm">A complete rebranding project including logo, typography, and visual guidelines.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="py-24 px-6 md:px-20 bg-white">
        <div class="max-w-5xl mx-auto rounded-[3rem] bg-slate-900 p-12 md:p-20 text-center text-white soft-shadow">
            <h2 class="text-4xl md:text-5xl font-extrabold mb-8">Ready to build something <span class="text-accent">extraordinary?</span></h2>
            <p class="text-slate-400 mb-12 text-lg">Send us a message and let's discuss your next project.</p>
            
            <div class="flex flex-col md:flex-row gap-6 justify-center">
                <a href="mailto:sulzadesign@hotmail.com" class="bg-accent text-slate-900 px-10 py-4 rounded-xl font-bold flex items-center justify-center gap-2 hover:scale-105 transition">
                    <i class="fa-solid fa-envelope"></i> Email Us
                </a>
                <a href="https://wa.me/2348149247947" class="bg-white/10 border border-white/20 px-10 py-4 rounded-xl font-bold flex items-center justify-center gap-2 hover:bg-white/20 transition">
                    <i class="fa-brands fa-whatsapp"></i> WhatsApp
                </a>
            </div>
        </div>
    </section>

    <footer class="py-12 px-6 text-center border-t border-slate-100">
        <p class="text-slate-400 text-sm mb-6">© 2026 Sulza Design Studio. All rights reserved.</p>
        <div class="flex justify-center gap-8 text-slate-400">
            <a href="#" class="hover:text-accent transition"><i class="fa-brands fa-linkedin-in"></i></a>
            <a href="#" class="hover:text-accent transition"><i class="fa-brands fa-github"></i></a>
            <a href="#" class="hover:text-accent transition"><i class="fa-brands fa-behance"></i></a>
        </div>
    </footer>

</body>
</html>
