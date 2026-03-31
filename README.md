<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JAE | Estrategia & Datos - Consultoría Premium</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,600;1,600&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        serif: ['"Playfair Display"', 'serif'],
                    },
                    colors: {
                        navy: {
                            900: '#0A1128',
                            800: '#121E3E',
                        },
                        copper: {
                            500: '#C5A059',
                            600: '#A38042',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom Styles for elegance */
        body {
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        .glass-nav {
            background: rgba(10, 17, 40, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        .hero-bg {
            background-image: linear-gradient(to right, rgba(10, 17, 40, 0.9), rgba(10, 17, 40, 0.7)), url('https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
        .fade-in-up {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        .fade-in-up.visible {
            opacity: 1;
            transform: translateY(0);
        }
        .service-card {
            transition: all 0.3s ease;
        }
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
            border-color: #C5A059;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans selection:bg-copper-500 selection:text-white">

    <!-- Navegación -->
    <nav class="fixed w-full z-50 glass-nav transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center cursor-pointer">
                    <span class="text-white font-serif text-2xl tracking-wider font-semibold">JAE</span>
                    <span class="text-gray-400 font-sans text-sm ml-3 tracking-widest uppercase hidden sm:block border-l border-gray-600 pl-3">Estrategia & Datos</span>
                </div>
                <!-- Menú Desktop -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#areas" class="text-gray-300 hover:text-white text-sm font-medium tracking-wide transition-colors">Áreas de Práctica</a>
                    <a href="#perfil" class="text-gray-300 hover:text-white text-sm font-medium tracking-wide transition-colors">Trayectoria</a>
                    <a href="#contacto" class="bg-copper-500 hover:bg-copper-600 text-white px-6 py-2.5 rounded text-sm font-semibold tracking-wide transition-all duration-300 shadow-lg shadow-copper-500/30">
                        Agendar Evaluación
                    </a>
                </div>
                <!-- Botón Móvil -->
                <div class="md:hidden flex items-center">
                    <button class="text-gray-300 hover:text-white focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative h-screen flex items-center hero-bg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 w-full pt-20">
            <div class="max-w-3xl observe fade-in-up">
                <div class="inline-flex items-center space-x-2 mb-6">
                    <span class="w-12 h-[1px] bg-copper-500"></span>
                    <span class="text-copper-500 uppercase tracking-widest text-xs font-bold">Consultoría Estratégica Premium</span>
                </div>
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-white leading-tight mb-6">
                    Escalabilidad y Soluciones Impulsadas por Datos.
                </h1>
                <p class="text-lg md:text-xl text-gray-300 mb-10 leading-relaxed font-light max-w-2xl">
                    Transformamos la complejidad operativa en crecimiento. Mediante análisis avanzado, identificamos la causa raíz de sus desafíos y ejecutamos soluciones estructuradas bajo estrictos SLAs y KPIs.
                </p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#contacto" class="bg-copper-500 hover:bg-copper-600 text-white px-8 py-4 rounded font-semibold tracking-wide text-center transition-all duration-300 shadow-lg shadow-copper-500/25">
                        Agendar Evaluación Operativa
                    </a>
                    <a href="#areas" class="border border-gray-500 text-white hover:border-white hover:bg-white/5 px-8 py-4 rounded font-semibold tracking-wide text-center transition-all duration-300">
                        Explorar Prácticas
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Proof / Barra de Confianza -->
    <div class="bg-navy-900 border-b border-gray-800 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <p class="text-center text-gray-400 text-sm uppercase tracking-widest mb-6">Experiencia comprobada en industrias de alta complejidad</p>
            <div class="flex flex-wrap justify-center items-center gap-8 md:gap-16 opacity-70">
                <span class="text-gray-300 font-serif italic text-lg">Finanzas & Inversiones</span>
                <span class="text-gray-300 font-serif italic text-lg">Telecomunicaciones</span>
                <span class="text-gray-300 font-serif italic text-lg">Educación Superior</span>
                <span class="text-gray-300 font-serif italic text-lg">Ecosistemas Fintech</span>
            </div>
        </div>
    </div>

    <!-- Áreas de Práctica -->
    <section id="areas" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16 observe fade-in-up">
                <h2 class="text-3xl md:text-4xl font-serif text-navy-900 mb-4">Soluciones Integrales para la Toma de Decisiones</h2>
                <div class="w-16 h-1 bg-copper-500 mx-auto mb-6"></div>
                <p class="text-gray-600">Enfoque metódico y estructurado para escalar operaciones, optimizar productos y maximizar la rentabilidad corporativa.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Servicio 1 -->
                <div class="service-card border border-gray-100 bg-gray-50 p-10 rounded-lg observe fade-in-up" style="transition-delay: 100ms;">
                    <div class="w-12 h-12 bg-navy-900 text-copper-500 rounded flex items-center justify-center mb-6">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"></path></svg>
                    </div>
                    <h3 class="text-xl font-bold text-navy-900 mb-3">Business Intelligence & Data Science</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">Diseño de paneles de gestión avanzados (Power BI) y modelos de anticipación de escenarios para transformar datos complejos en acciones ejecutivas inmediatas e identificar la causa raíz de ineficiencias.</p>
                </div>

                <!-- Servicio 2 -->
                <div class="service-card border border-gray-100 bg-gray-50 p-10 rounded-lg observe fade-in-up" style="transition-delay: 200ms;">
                    <div class="w-12 h-12 bg-navy-900 text-copper-500 rounded flex items-center justify-center mb-6">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"></path></svg>
                    </div>
                    <h3 class="text-xl font-bold text-navy-900 mb-3">PMO y Transformación Operativa</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">Liderazgo metódico en la coordinación de proyectos tecnológicos e integraciones complejas. Aseguramos el cumplimiento de plazos y métricas de éxito (SLAs/KPIs) alineando tecnología con el negocio.</p>
                </div>

                <!-- Servicio 3 -->
                <div class="service-card border border-gray-100 bg-gray-50 p-10 rounded-lg observe fade-in-up" style="transition-delay: 300ms;">
                    <div class="w-12 h-12 bg-navy-900 text-copper-500 rounded flex items-center justify-center mb-6">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"></path></svg>
                    </div>
                    <h3 class="text-xl font-bold text-navy-900 mb-3">Estrategia Corporativa & Finanzas</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">Asesoría de alto nivel para evaluar la viabilidad financiera, estructurar modelos de negocio y escalar productos. Visión transversal y estratégica orientada a maximizar el rendimiento.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Perfil / Autoridad -->
    <section id="perfil" class="py-24 bg-gray-50 border-t border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col lg:flex-row items-center gap-16">
                <!-- Imagen -->
                <div class="w-full lg:w-5/12 observe fade-in-up">
                    <div class="relative">
                        <div class="absolute -inset-4 bg-copper-500/20 transform translate-x-4 translate-y-4 rounded"></div>
                        <!-- Placeholder de imagen: Reemplazar src con la foto real -->
                        <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?q=80&w=1974&auto=format&fit=crop" alt="Juan Andrés Escobar" class="relative z-10 w-full h-auto object-cover rounded shadow-2xl grayscale hover:grayscale-0 transition-all duration-500">
                    </div>
                </div>
                <!-- Texto -->
                <div class="w-full lg:w-7/12 observe fade-in-up" style="transition-delay: 200ms;">
                    <span class="text-copper-600 font-bold tracking-widest uppercase text-xs mb-2 block">Director & Consultor Estratégico</span>
                    <h2 class="text-3xl md:text-4xl font-serif text-navy-900 mb-6">Juan Andrés Escobar H.</h2>
                    
                    <div class="space-y-4 text-gray-600 mb-8">
                        <p>
                            Con más de 10 años de trayectoria multidisciplinaria, mi enfoque combina el rigor metodológico de la Ingeniería Informática con una visión financiera aguda.
                        </p>
                        <p>
                            Como Magíster en Finanzas y especialista en Business Intelligence, he liderado transformaciones operativas desde la vicerrectoría de instituciones de educación superior hasta la dirección ejecutiva de startups Fintech y empresas de tecnología.
                        </p>
                        <p class="font-medium text-navy-900 border-l-4 border-copper-500 pl-4 py-1 italic">
                            "Mi compromiso es claro: decisiones metódicas, orientadas al logro y siempre respaldadas por evidencia."
                        </p>
                    </div>

                    <a href="https://linkedin.com" target="_blank" class="inline-flex items-center text-navy-900 font-semibold hover:text-copper-600 transition-colors">
                        Conectar en LinkedIn
                        <svg class="w-5 h-5 ml-2" fill="currentColor" viewBox="0 0 24 24"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer / Contacto -->
    <footer id="contacto" class="bg-navy-900 text-gray-300 py-16 border-t-[6px] border-copper-500">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
                <!-- Branding -->
                <div>
                    <div class="flex items-center mb-6">
                        <span class="text-white font-serif text-3xl tracking-wider font-semibold">JAE</span>
                    </div>
                    <p class="text-sm text-gray-400 max-w-xs leading-relaxed">
                        Escalabilidad y soluciones estratégicas impulsadas por datos para empresas de alta complejidad.
                    </p>
                </div>
                
                <!-- Contact Info -->
                <div>
                    <h4 class="text-white font-semibold uppercase tracking-widest text-xs mb-6">Contacto Directo</h4>
                    <ul class="space-y-4 text-sm">
                        <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 text-copper-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                            <a href="mailto:jaescobar.h@gmail.com" class="hover:text-white transition-colors">jaescobar.h@gmail.com</a>
                        </li>
                        <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 text-copper-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path></svg>
                            <a href="tel:+56993066366" class="hover:text-white transition-colors">+56 9 9306 6366</a>
                        </li>
                        <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 text-copper-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
                            <span>Vitacura, Santiago, Chile.</span>
                        </li>
                    </ul>
                </div>

                <!-- Links Legales -->
                <div>
                    <h4 class="text-white font-semibold uppercase tracking-widest text-xs mb-6">Información</h4>
                    <ul class="space-y-3 text-sm">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Políticas de Privacidad</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Términos de Servicio</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Portal de Clientes</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 text-center text-xs text-gray-500 flex flex-col sm:flex-row justify-between items-center">
                <p>&copy; 2026 JAE Estrategia & Datos. Todos los derechos reservados.</p>
                <p class="mt-2 sm:mt-0">Diseñado con rigor y precisión.</p>
            </div>
        </div>
    </footer>

    <!-- Interacciones JS simples para scroll y navbar -->
    <script>
        // Navbar bg on scroll
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.classList.add('shadow-lg');
                nav.style.background = 'rgba(10, 17, 40, 0.98)';
            } else {
                nav.classList.remove('shadow-lg');
                nav.style.background = 'rgba(10, 17, 40, 0.8)';
            }
        });

        // Intersection Observer for fade-in animations
        const observerOptions = {
            root: null,
            rootMargin: '0px',
            threshold: 0.15
        };

        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);

        document.querySelectorAll('.observe').forEach(element => {
            observer.observe(element);
        });
    </script>
</body>
</html>
