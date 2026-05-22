
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Daniel Torrealba · Dev Portfolio</title>
    <!-- Tailwind CSS v3 + Font Awesome + Google Fonts (Inter) -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Personalizar la configuración de Tailwind para un look más profesional -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'sans': ['Inter', 'system-ui', 'Segoe UI', 'Roboto', 'sans-serif'],
                    },
                    colors: {
                        'primary': '#0f172a',
                        'secondary': '#3b82f6',
                        'accent': '#0ea5e9',
                        'dark-card': '#1e293b',
                    },
                    animation: {
                        'fade-in': 'fadeIn 0.8s ease-out',
                        'slide-up': 'slideUp 0.5s ease-out',
                        'float': 'float 6s ease-in-out infinite',
                    },
                    keyframes: {
                        fadeIn: { '0%': { opacity: '0' }, '100%': { opacity: '1' } },
                        slideUp: { '0%': { transform: 'translateY(20px)', opacity: '0' }, '100%': { transform: 'translateY(0)', opacity: '1' } },
                        float: { '0%': { transform: 'translateY(0px)' }, '50%': { transform: 'translateY(-10px)' }, '100%': { transform: 'translateY(0px)' } },
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Smooth scroll y mejoras sutiles */
        html { scroll-behavior: smooth; }
        body { background: linear-gradient(135deg, #f8fafc 0%, #eef2ff 100%); }
        .glass-card { backdrop-filter: blur(2px); background: rgba(255,255,255,0.7); border: 1px solid rgba(255,255,255,0.5); }
        .gradient-border {
            background: linear-gradient(90deg, #3b82f6, #06b6d4, #8b5cf6);
            background-size: 200% 200%;
            animation: gradientShift 4s ease infinite;
        }
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .hover-lift { transition: all 0.25s ease; }
        .hover-lift:hover { transform: translateY(-4px); box-shadow: 0 20px 25px -12px rgba(0,0,0,0.1); }
        code { font-family: 'JetBrains Mono', monospace; background: #eef2ff; padding: 0.2rem 0.4rem; border-radius: 0.5rem; font-size: 0.85rem; }
        .tech-badge { transition: all 0.2s; }
        .tech-badge:hover { transform: scale(1.05); filter: brightness(1.05); }
    </style>
</head>
<body class="font-sans antialiased">

    <!-- Contenedor principal con max-width elegante y centrado -->
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 py-10 md:py-14 animate-fade-in">
        
        <!-- Header / Hero Section -->
        <div class="text-center mb-14 md:mb-20">
            <div class="inline-block mb-4 p-1 rounded-full bg-gradient-to-r from-blue-500 to-cyan-400 shadow-md">
                <div class="bg-white rounded-full p-1">
                    <img src="https://ui-avatars.com/api/?background=0f172a&color=fff&bold=true&size=100&name=Daniel+Torrealba&fontsize=0.45&rounded=true" alt="Daniel Torrealba" class="w-24 h-24 rounded-full shadow-md">
                </div>
            </div>
            <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-slate-800 to-slate-600">Daniel Torrealba</h1>
            <div class="mt-4 flex flex-wrap items-center justify-center gap-2 text-slate-600">
                <span class="inline-flex items-center gap-1.5 bg-white/60 backdrop-blur-sm px-4 py-1.5 rounded-full text-sm font-medium shadow-sm"><i class="fas fa-code text-blue-500"></i> Desarrollador Full-Stack</span>
                <span class="inline-flex items-center gap-1.5 bg-white/60 backdrop-blur-sm px-4 py-1.5 rounded-full text-sm font-medium shadow-sm"><i class="fas fa-chart-line text-emerald-500"></i> Analista de Sistemas</span>
                <span class="inline-flex items-center gap-1.5 bg-white/60 backdrop-blur-sm px-4 py-1.5 rounded-full text-sm font-medium shadow-sm"><i class="fas fa-laptop-code text-indigo-500"></i> TSU en Informática</span>
            </div>
            <div class="mt-6 flex justify-center">
                <div class="inline-flex items-center gap-2 bg-slate-800/90 text-white px-4 py-1.5 rounded-full text-sm shadow-md backdrop-blur-sm">
                    <i class="fas fa-eye text-blue-300"></i>
                    <span>Visitas al perfil: <strong>1,284</strong></span>
                    <i class="far fa-clock ml-2 text-blue-300"></i>
                    <span>Activo · 2025</span>
                </div>
            </div>
            <!-- línea decorativa -->
            <div class="w-24 h-1 gradient-border rounded-full mx-auto mt-8"></div>
        </div>

        <!-- Sobre mí - Sección profesional -->
        <div class="bg-white/80 backdrop-blur-sm rounded-2xl shadow-xl p-6 md:p-8 mb-12 border border-white/40 hover-lift transition-all">
            <div class="flex items-center gap-3 mb-5">
                <div class="p-2 bg-blue-100 rounded-xl text-blue-700"><i class="fas fa-user-astronaut text-2xl"></i></div>
                <h2 class="text-2xl md:text-3xl font-bold text-slate-800">🚀 Sobre mí</h2>
            </div>
            <p class="text-slate-700 leading-relaxed text-base md:text-lg">
                Como <strong class="text-blue-700">Técnico Superior Universitario en Informática</strong> y Analista de Sistemas, combino formación académica sólida con <strong class="text-blue-700">experiencia comprobada</strong> en desarrollo web y soluciones empresariales.  
                Mi enfoque principal es diseñar arquitecturas escalables bajo el patrón <strong class="bg-blue-50 px-1.5 py-0.5 rounded">MVC</strong> para optimizar procesos de negocio y generar valor real.  
                Actualmente expandiendo conocimientos en infraestructura moderna y preparándome para nuevas certificaciones tecnológicas, mientras desarrollo software a medida que transforma ideas en productos digitales.
            </p>
            <div class="mt-5 flex flex-wrap gap-2">
                <span class="text-xs bg-slate-100 text-slate-600 px-3 py-1 rounded-full"><i class="far fa-check-circle text-green-500 mr-1"></i>Metodologías ágiles</span>
                <span class="text-xs bg-slate-100 text-slate-600 px-3 py-1 rounded-full"><i class="fas fa-brain text-purple-500 mr-1"></i>Resolución analítica</span>
                <span class="text-xs bg-slate-100 text-slate-600 px-3 py-1 rounded-full"><i class="fas fa-rocket text-cyan-500 mr-1"></i>Entregas incrementales</span>
            </div>
        </div>

        <!-- Stack Tecnológico moderno (eliminado Cisco) -->
        <div class="mb-12">
            <div class="flex items-center justify-between flex-wrap gap-3 mb-7">
                <div class="flex items-center gap-3">
                    <div class="p-2 bg-indigo-100 rounded-xl text-indigo-700"><i class="fas fa-layer-group text-2xl"></i></div>
                    <h2 class="text-2xl md:text-3xl font-bold text-slate-800">💻 Stack Tecnológico</h2>
                </div>
                <span class="text-xs text-slate-500 bg-white/50 px-3 py-1.5 rounded-full"><i class="fas fa-microchip"></i> Ecosistema full-stack</span>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Frontend Column -->
                <div class="bg-white/70 rounded-xl p-5 shadow-sm border border-gray-100 hover:shadow-md transition">
                    <div class="flex items-center gap-2 mb-4 border-b border-gray-200 pb-2">
                        <i class="fab fa-react text-blue-500 text-xl"></i>
                        <h3 class="font-semibold text-xl text-slate-700">Frontend</h3>
                    </div>
                    <div class="flex flex-wrap gap-3">
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#E34F26]/10 text-[#E34F26] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-html5"></i> HTML5</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#1572B6]/10 text-[#1572B6] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-css3-alt"></i> CSS3</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#F7DF1E]/20 text-[#E5A81C] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-js"></i> JavaScript</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#61DAFB]/20 text-[#0C4E6F] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-react"></i> React</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#06B6D4]/10 text-[#0E7490] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-tailwind"></i> Tailwind CSS</span>
                    </div>
                </div>
                
                <!-- Backend & DB Column -->
                <div class="bg-white/70 rounded-xl p-5 shadow-sm border border-gray-100 hover:shadow-md transition">
                    <div class="flex items-center gap-2 mb-4 border-b border-gray-200 pb-2">
                        <i class="fas fa-database text-emerald-600 text-xl"></i>
                        <h3 class="font-semibold text-xl text-slate-700">Backend & Bases de Datos</h3>
                    </div>
                    <div class="flex flex-wrap gap-3">
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#777BB4]/20 text-[#5A5D8F] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-php"></i> PHP</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#FF2D20]/20 text-[#C92C1E] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-laravel"></i> Laravel</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#3776AB]/20 text-[#2D5F8B] px-4 py-2 rounded-full text-sm font-medium"><i class="fab fa-python"></i> Python</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-[#4479A1]/20 text-[#2C5E7A] px-4 py-2 rounded-full text-sm font-medium"><i class="fas fa-database"></i> MySQL</span>
                        <span class="tech-badge inline-flex items-center gap-2 bg-gray-200 text-gray-700 px-4 py-2 rounded-full text-sm font-medium"><i class="fas fa-server"></i> REST APIs</span>
                    </div>
                </div>
            </div>
            <!-- Infraestructura / Redes simplificado, sin mención a Cisco, solo herramientas modernas -->
            <div class="mt-6 bg-white/70 rounded-xl p-5 shadow-sm border border-gray-100">
                <div class="flex items-center gap-2 mb-3">
                    <i class="fas fa-cloud-upload-alt text-slate-600 text-xl"></i>
                    <h3 class="font-semibold text-xl text-slate-700">DevOps & Herramientas</h3>
                </div>
                <div class="flex flex-wrap gap-3">
                    <span class="bg-slate-100 text-slate-700 px-4 py-2 rounded-full text-sm"><i class="fab fa-git-alt"></i> Git/GitHub</span>
                    <span class="bg-slate-100 text-slate-700 px-4 py-2 rounded-full text-sm"><i class="fas fa-terminal"></i> CLI · Bash</span>
                    <span class="bg-slate-100 text-slate-700 px-4 py-2 rounded-full text-sm"><i class="fas fa-network-wired"></i> Redes / TCP/IP</span>
                    <span class="bg-slate-100 text-slate-700 px-4 py-2 rounded-full text-sm"><i class="fas fa-vial"></i> Testing & Debugging</span>
                </div>
            </div>
        </div>
        
        <!-- Proyectos Destacados (Glassmorphism profesional) -->
        <div class="mb-14">
            <div class="flex items-center gap-3 mb-7">
                <div class="p-2 bg-amber-100 rounded-xl text-amber-700"><i class="fas fa-diagram-project text-2xl"></i></div>
                <h2 class="text-2xl md:text-3xl font-bold text-slate-800">📂 Proyectos Destacados</h2>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Card 1 -->
                <div class="group bg-white/70 backdrop-blur-sm rounded-2xl p-5 shadow-md hover:shadow-xl transition-all duration-300 border border-white/50 hover:border-blue-200">
                    <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-blue-500 to-cyan-400 flex items-center justify-center mb-4 shadow-md group-hover:scale-105 transition">
                        <i class="fas fa-ticket-alt text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Tyxflow</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Sistema web integral de mesa de ayuda (Helpdesk) y gestión de tickets para soporte técnico. Optimización de flujos SLA.</p>
                    <div class="mt-3 flex gap-1 text-xs text-blue-600"><i class="fas fa-code-branch"></i> Laravel · MySQL · Livewire</div>
                </div>
                <!-- Card 2 -->
                <div class="group bg-white/70 backdrop-blur-sm rounded-2xl p-5 shadow-md hover:shadow-xl transition-all duration-300 border border-white/50 hover:border-emerald-200">
                    <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-emerald-500 to-teal-400 flex items-center justify-center mb-4 shadow-md group-hover:scale-105 transition">
                        <i class="fas fa-hotel text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Sistema Hotelero</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Plataforma robusta para administración centralizada de reservas, control operativo, facturación y reportes en tiempo real.</p>
                    <div class="mt-3 flex gap-1 text-xs text-emerald-600"><i class="fas fa-chart-line"></i> PHP · React · PostgreSQL</div>
                </div>
                <!-- Card 3 -->
                <div class="group bg-white/70 backdrop-blur-sm rounded-2xl p-5 shadow-md hover:shadow-xl transition-all duration-300 border border-white/50 hover:border-purple-200">
                    <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-purple-500 to-pink-400 flex items-center justify-center mb-4 shadow-md group-hover:scale-105 transition">
                        <i class="fas fa-chart-simple text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-slate-800">Inventario + Ventas</h3>
                    <p class="text-slate-600 text-sm mt-2 leading-relaxed">Aplicación de escritorio en Python orientada a emprendedores. Gestión de stock, facturación y dashboards inteligentes.</p>
                    <div class="mt-3 flex gap-1 text-xs text-purple-600"><i class="fab fa-python"></i> Python · Tkinter · SQLite</div>
                </div>
            </div>
        </div>

        <!-- Propuesta de Valor + Competencias (Grid 2x2 atractiva) -->
        <div class="mb-14">
            <div class="flex items-center gap-3 mb-7">
                <div class="p-2 bg-violet-100 rounded-xl text-violet-700"><i class="fas fa-gem text-2xl"></i></div>
                <h2 class="text-2xl md:text-3xl font-bold text-slate-800">🎯 Propuesta de Valor</h2>
            </div>
            <div class="grid md:grid-cols-2 gap-5">
                <div class="bg-white/60 p-5 rounded-xl shadow-sm flex gap-4 items-start border-l-4 border-blue-500">
                    <i class="fas fa-cubes text-3xl text-blue-500"></i>
                    <div><h3 class="font-bold text-lg">Arquitectura modular</h3><p class="text-slate-600 text-sm">Código mantenible, escalable y con patrones de diseño sólidos orientados a resultados de negocio.</p></div>
                </div>
                <div class="bg-white/60 p-5 rounded-xl shadow-sm flex gap-4 items-start border-l-4 border-emerald-500">
                    <i class="fas fa-eye text-3xl text-emerald-500"></i>
                    <div><h3 class="font-bold text-lg">Visión integral</h3><p class="text-slate-600 text-sm">Desde base de datos, lógica backend hasta UI/UX e infraestructura de red.</p></div>
                </div>
                <div class="bg-white/60 p-5 rounded-xl shadow-sm flex gap-4 items-start border-l-4 border-amber-500">
                    <i class="fas fa-lightbulb text-3xl text-amber-500"></i>
                    <div><h3 class="font-bold text-lg">Resolución de problemas</h3><p class="text-slate-600 text-sm">Anticipación a fallos, mejoras continuas y entregas de alta calidad bajo presión.</p></div>
                </div>
                <div class="bg-white/60 p-5 rounded-xl shadow-sm flex gap-4 items-start border-l-4 border-purple-500">
                    <i class="fas fa-rocket text-3xl text-purple-500"></i>
                    <div><h3 class="font-bold text-lg">Adaptabilidad rápida</h3><p class="text-slate-600 text-sm">Integración ágil a equipos, metodologías agiles y adopción de tecnologías emergentes.</p></div>
                </div>
            </div>
        </div>

        <!-- Formación profesional + certificaciones -->
        <div class="mb-14 bg-slate-800/5 rounded-2xl p-6 md:p-8 backdrop-blur-sm border border-slate-200">
            <div class="flex flex-wrap items-center justify-between gap-4 mb-5">
                <div class="flex items-center gap-3">
                    <i class="fas fa-graduation-cap text-3xl text-slate-700"></i>
                    <h2 class="text-2xl md:text-3xl font-bold text-slate-800">🎓 Formación Profesional</h2>
                </div>
                <span class="text-xs bg-white/80 px-3 py-1 rounded-full"><i class="fas fa-certificate"></i> Actualización continua</span>
            </div>
            <div class="flex flex-wrap gap-6 justify-between items-center">
                <div class="flex items-center gap-4">
                    <div class="bg-white p-3 rounded-full shadow"><i class="fas fa-university text-3xl text-blue-700"></i></div>
                    <div><p class="font-bold text-lg">Técnico Superior Universitario en Informática</p><p class="text-slate-600 text-sm">Especialización en análisis, desarrollo y arquitectura de software</p></div>
                </div>
                <div class="w-px h-12 bg-slate-300 hidden md:block"></div>
                <div class="flex items-center gap-4">
                    <div class="bg-white p-3 rounded-full shadow"><i class="fas fa-chalkboard-user text-3xl text-emerald-700"></i></div>
                    <div><p class="font-bold text-lg">Analista de Sistemas</p><p class="text-slate-600 text-sm">Optimización de procesos, levantamiento de requerimientos y diseño funcional</p></div>
                </div>
                <div class="w-px h-12 bg-slate-300 hidden md:block"></div>
                <div class="flex items-center gap-4">
                    <div class="bg-white p-3 rounded-full shadow"><i class="fas fa-certificate text-3xl text-amber-600"></i></div>
                    <div><p class="font-bold text-lg">Certificaciones en curso</p><p class="text-slate-600 text-sm">Cloud · Seguridad · Arquitectura avanzada</p></div>
                </div>
            </div>
        </div>
        
        <!-- Footer con contacto / redes sociales profesionales -->
        <div class="text-center pt-6 border-t border-slate-200 mt-4">
            <div class="flex flex-wrap justify-center gap-5 text-slate-500 mb-4">
                <a href="#" class="hover:text-blue-600 transition transform hover:scale-110 inline-flex items-center gap-2"><i class="fab fa-github text-xl"></i> GitHub</a>
                <a href="#" class="hover:text-blue-600 transition transform hover:scale-110 inline-flex items-center gap-2"><i class="fab fa-linkedin text-xl"></i> LinkedIn</a>
                <a href="#" class="hover:text-blue-600 transition transform hover:scale-110 inline-flex items-center gap-2"><i class="fas fa-envelope text-xl"></i> daniel.t@dev.com</a>
                <a href="#" class="hover:text-blue-600 transition transform hover:scale-110 inline-flex items-center gap-2"><i class="fas fa-portrait text-xl"></i> Portfolio</a>
            </div>
            <p class="text-xs text-slate-400 mt-3">Construyendo soluciones escalables con pasión por el código limpio y la arquitectura eficiente.</p>
            <p class="text-xs text-slate-300 mt-1">© 2025 Daniel Torrealba — Actualizado con Tailwind CSS</p>
        </div>
    </div>
</body>
</html>
