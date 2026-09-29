<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="CODEX BELLATOR - ARS UNIFIED. Ciencia de Combate Unificado. Sistema de alta ingeniería humana, neurofisiología aplicada y telemetría biológica.">
    <title>CODEX BELLATOR - ARS UNIFIED | Ciencia de Combate Unificado</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        gold: {
                            50: '#fffbeb',
                            100: '#fef3c7',
                            400: '#fbbf24',
                            500: '#f59e0b',
                            600: '#d97706',
                            700: '#b45309',
                        },
                        amberGold: '#d4af37',
                        tactical: {
                            900: '#0b0f19',
                            800: '#111827',
                            700: '#1f2937',
                            600: '#374151',
                            accent: '#f59e0b',
                            cyan: '#06b6d4',
                            red: '#ef4444'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace']
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0b0f19;
            color: #f3f4f6;
        }
        .glow-amber {
            box-shadow: 0 0 25px -5px rgba(245, 158, 11, 0.3);
        }
        .glow-cyan {
            box-shadow: 0 0 25px -5px rgba(6, 182, 212, 0.3);
        }
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0b0f19;
        }
        ::-webkit-scrollbar-thumb {
            background: #374151;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #f59e0b;
        }
    </style>
</head>
<body class="bg-tactical-900 text-gray-100 antialiased selection:bg-amber-500 selection:text-black overflow-x-hidden">

    <!-- Sticky Navigation Header -->
    <header class="sticky top-0 z-50 bg-tactical-900/90 backdrop-blur-md border-b border-tactical-700/60 transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-9 h-9 rounded-lg bg-gradient-to-br from-amber-500 to-amber-700 flex items-center justify-center text-black font-black text-lg group-hover:scale-105 transition-transform">
                    <i class="fa-solid fa-shield-halved"></i>
                </div>
                <div>
                    <span class="font-bold tracking-wider text-sm sm:text-base text-gray-100 block leading-none">CODEX BELLATOR</span>
                    <span class="text-xs text-amber-500 font-mono tracking-widest block leading-tight">ARS UNIFIED</span>
                </div>
            </a>

            <!-- Quick Navigation Links -->
            <nav class="hidden lg:flex items-center gap-5 text-xs font-semibold tracking-wider uppercase text-gray-300">
                <a href="#que-es" class="hover:text-amber-400 transition-colors">¿Qué es?</a>
                <a href="#para-que-sirve" class="hover:text-amber-400 transition-colors">¿Para qué sirve?</a>
                <a href="#objetivo" class="hover:text-amber-400 transition-colors">Objetivo</a>
                <a href="#como-funciona" class="hover:text-amber-400 transition-colors">Funcionamiento</a>
                <a href="#realmente-funciona" class="hover:text-amber-400 transition-colors">Evidencia</a>
                <a href="#diferencias" class="hover:text-amber-400 transition-colors">Comparativa</a>
                <a href="#redes" class="hover:text-amber-400 transition-colors">Redes</a>
                <a href="#descarga" class="hover:text-amber-400 transition-colors text-amber-400">Descarga</a>
            </nav>

            <div class="flex items-center gap-3">
                <a href="#conocer" class="px-4 py-2 text-xs font-bold uppercase tracking-wider bg-amber-500 text-black rounded-lg hover:bg-amber-400 transition-all shadow-lg shadow-amber-500/20 flex items-center gap-2">
                    <i class="fa-solid fa-book-bookmark"></i>
                    <span class="hidden sm:inline">Explorar Codex</span>
                </a>
                <button id="mobile-menu-btn" aria-label="Abrir menú" class="lg:hidden p-2 text-gray-400 hover:text-white">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile dropdown menu -->
        <div id="mobile-menu" class="hidden lg:hidden bg-tactical-800 border-b border-tactical-700 px-4 py-4 space-y-3 text-sm">
            <a href="#que-es" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">¿Qué es el Codex?</a>
            <a href="#para-que-sirve" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">¿Para qué sirve?</a>
            <a href="#objetivo" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">¿Cuál es su objetivo?</a>
            <a href="#como-funciona" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">¿Cómo funciona?</a>
            <a href="#realmente-funciona" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">¿Realmente funciona?</a>
            <a href="#diferencias" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">Diferencias Metodológicas</a>
            <a href="#redes" class="block text-gray-300 hover:text-amber-400 font-medium mobile-link">Canales Oficiales</a>
            <a href="#descarga" class="block text-amber-400 hover:text-amber-300 font-bold mobile-link">Descargar Codex Completo</a>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative pt-12 pb-16 px-4 sm:px-6 lg:px-8 max-w-5xl mx-auto text-center" id="conocer">
        <div class="absolute inset-0 -z-10 bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-amber-500/10 via-tactical-900/60 to-transparent"></div>
        
        <div class="border-2 border-amber-500/80 bg-tactical-800/90 rounded-2xl p-6 sm:p-10 md:p-12 shadow-2xl glow-amber relative overflow-hidden backdrop-blur-sm">
            <div class="absolute top-0 right-0 w-32 h-32 bg-amber-500/10 rounded-full blur-2xl pointer-events-none"></div>
            <div class="absolute bottom-0 left-0 w-32 h-32 bg-cyan-500/10 rounded-full blur-2xl pointer-events-none"></div>

            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-amber-500/10 border border-amber-500/30 text-amber-400 text-xs font-mono mb-6">
                <span class="w-2 h-2 rounded-full bg-amber-400 animate-pulse"></span>
                Marco de Validación Doctrinal | C.C.U.
            </div>

            <h1 class="text-3xl sm:text-5xl md:text-6xl font-black tracking-tight text-white uppercase mb-3 leading-tight">
                CODEX BELLATOR
            </h1>
            <h2 class="text-xl sm:text-2xl md:text-3xl font-extrabold text-amber-400 tracking-wider uppercase mb-4 font-mono leading-tight">
                ARS UNIFIED
            </h2>
            <p class="text-lg sm:text-xl text-gray-300 font-medium mb-8 max-w-2xl mx-auto">
                Ciencia de Combate Unificado
            </p>

            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <a href="#que-es" class="w-full sm:w-auto px-8 py-4 bg-amber-500 hover:bg-amber-400 text-black font-black uppercase tracking-widest text-sm rounded-xl transition-all shadow-xl hover:scale-105 flex items-center justify-center gap-3">
                    <span>[ CONOCER EL CODEX ]</span>
                    <i class="fa-solid fa-arrow-down"></i>
                </a>
                <a href="#descarga" class="w-full sm:w-auto px-6 py-4 bg-tactical-700 hover:bg-tactical-600 text-amber-400 font-bold uppercase tracking-wider text-sm rounded-xl transition-all border border-amber-500/30 flex items-center justify-center gap-2">
                    <i class="fa-solid fa-file-pdf"></i>
                    <span>Documento Completo</span>
                </a>
            </div>

            <div class="mt-8 pt-6 border-t border-tactical-700/80 flex flex-wrap justify-center gap-4 text-xs text-gray-400 font-mono">
                <span><i class="fa-solid fa-shield text-amber-500 mr-1"></i>Arquitectura Metodológica Canónica</span>
                <span>•</span>
                <span><i class="fa-solid fa-code-branch text-amber-500 mr-1"></i>Doctrina Versión 4.0</span>
            </div>
        </div>
    </section>

    <!-- SECTION 1: ¿QUÉ ES? -->
    <section id="que-es" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">1</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿QUÉ ES EL CODEX BELLATOR ARS UNIFIED?</h2>
            </div>
            <div class="prose prose-invert max-w-none text-gray-300 text-base sm:text-lg leading-relaxed space-y-6">
                <p class="font-medium text-amber-200/90 text-lg sm:text-xl border-l-4 border-amber-500 pl-4 py-1">
                    El <strong>Codex Bellator – Ars Unified</strong> es la <strong>Ciencia de Combate Unificado (C.C.U.)</strong>: un sistema cerrado de alta ingeniería humana, neurofisiología aplicada, biomecánica y telemetría biológica concebido para eliminar la entropía metodológica y los sesgos empíricos tradicionales.
                </p>
                <p>
                    Su propósito fundamental es transformar al practicante en un operador táctico capaz de anular la latencia reactiva, interpretar microseñales corporales y ejecutar intercepciones precisas en <strong>Tiempo Cero (T0)</strong>.
                </p>
            </div>
        </div>
    </section>

    <!-- SECTION 2: ¿PARA QUÉ SIRVE? -->
    <section id="para-que-sirve" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">2</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿PARA QUÉ SIRVE?</h2>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 flex gap-4">
                    <div class="text-amber-500 text-2xl shrink-0"><i class="fa-solid fa-stopwatch-20"></i></div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Anulación de Latencia Reactiva</h3>
                        <p class="text-xs sm:text-sm text-gray-400">Permite detectar microseñales y vectores de intención antes de que el golpe o derribo madure, disparando la respuesta en la génesis.</p>
                    </div>
                </div>
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 flex gap-4">
                    <div class="text-cyan-400 text-2xl shrink-0"><i class="fa-solid fa-shield-virus"></i></div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Protección del Chasis y Eficiencia</h3>
                        <p class="text-xs sm:text-sm text-gray-400">Mediante el Umbral de Velocidad Crítica (UVC 10%), erradica el volumen de entrenamiento basura, previniendo lesiones articulares y sobrecargas del S.N.C.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION 3: ¿CUÁL ES SU OBJETIVO? -->
    <section id="objetivo" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">3</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿CUÁL ES SU OBJETIVO?</h2>
            </div>
            <p class="text-gray-300 text-base leading-relaxed">
                Alcanzar la <span class="text-amber-400 font-bold">Soberanía Neural y la Inevitabilidad Táctica</span>, dominando de manera absoluta el espacio-tiempo del combate (Kairós) y maximizando la rentabilidad biológica de cada sesión de entrenamiento físico y técnico.
            </p>
        </div>
    </section>

    <!-- SECTION 4: ¿CÓMO FUNCIONA? -->
    <section id="como-funciona" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">4</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿CÓMO FUNCIONA?</h2>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-3 gap-2 border-b border-tactical-700 pb-4" role="tablist">
                <button data-target="content-vafp" role="tab" aria-selected="true" class="tab-btn active px-3 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-amber-500 text-black shadow-md">1. Motor V.A.F.P.</button>
                <button data-target="content-pfm" role="tab" aria-selected="false" class="tab-btn px-3 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300">2. Principios P.F.M.</button>
                <button data-target="content-lazo" role="tab" aria-selected="false" class="tab-btn px-3 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300">3. CNS & M.C.C.</button>
            </div>
            <div id="tab-content" class="bg-tactical-900/90 rounded-xl p-6 border border-tactical-700/80 mt-4">
                <div id="content-vafp" class="tab-pane space-y-4" role="tabpanel">
                    <h3 class="text-lg font-bold text-amber-400">Vector de Anticipación Fisiológica Proyectiva (V.A.F.P.)</h3>
                    <p class="text-sm text-gray-300">Interfaz neurobiológica encargada de comprimir el tiempo de procesamiento cognitivo, permitiendo lecturas de trayectorias y contramedidas automatizadas en milisegundos.</p>
                </div>
                <div id="content-pfm" class="tab-pane hidden space-y-4" role="tabpanel">
                    <h3 class="text-lg font-bold text-cyan-400">Principios Fundamentales del Movimiento (P.F.M.)</h3>
                    <p class="text-sm text-gray-300">Leyes físicas y mecánicas rectoras que gobiernan la geometría corporal, palancas y transferencia óptima de energía cinética en striking y grappling.</p>
                </div>
                <div id="content-lazo" class="tab-pane hidden space-y-4" role="tabpanel">
                    <h3 class="text-lg font-bold text-amber-400">C.N.S. & M.C.C.</h3>
                    <p class="text-sm text-gray-300">Arquitectura de control dinámico que supervisa el sistema nervioso central y ejecuta el Mecanismo de Compensación Continua para corregir fallos estructurales antes del colapso.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION 5: ¿REALMENTE FUNCIONA? -->
    <section id="realmente-funciona" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">5</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿REALMENTE FUNCIONA?</h2>
            </div>
            <div class="bg-tactical-900/90 rounded-2xl p-6 border border-amber-500/40 glow-amber">
                <h3 class="font-bold text-white text-base mb-2"><i class="fa-solid fa-calculator text-amber-400 mr-2"></i>Simulador S.M.V. (Cálculo IGD)</h3>
                <p class="text-xs text-gray-400 mb-4">Ajuste los valores de software técnico para comprobar el índice global y verificar la cláusula de voto de censura doctrinal:</p>
                <div class="space-y-3">
                    <div>
                        <div class="flex justify-between text-xs font-mono mb-1">
                            <span class="text-gray-300">Software Técnico (ST)</span>
                            <span id="val-st" class="text-amber-400 font-bold">4.5</span>
                        </div>
                        <input type="range" id="input-st" min="1" max="10" step="0.5" value="4.5" class="igd-input w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                    </div>
                </div>
                <div id="status-box" class="p-3 rounded-xl border mt-4 bg-red-500/20 border-red-500 text-red-300 text-center text-xs font-mono">
                    PROGRESIÓN BLOQUEADA: Voto de Censura Activo (ST < 5.0)
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION 6: DIFERENCIAS METODOLÓGICAS -->
    <section id="diferencias" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">6</div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">¿QUÉ LO DIFERENCIA?</h2>
            </div>
            <p class="text-gray-300 text-base leading-relaxed">
                A diferencia de los métodos tradicionales empíricos y secuenciales basados en repetición ciega y alta latencia, el <strong>Codex Bellator</strong> opera en paralelo bajo esquemas de telemetría y auditorías cuantitativas objetivas, garantizando adaptabilidad y precisión quirúrgica.
            </p>
        </div>
    </section>

    <!-- NUEVO APARTADO: REDES SOCIALES Y CANALES OFICIALES -->
    <section id="redes" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/80 border-2 border-amber-500/60 rounded-2xl p-6 sm:p-10 shadow-xl text-center">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-amber-500/20 border border-amber-500/40 text-amber-400 text-xs font-mono mb-4">
                <i class="fa-solid fa-satellite-dish"></i> Transmisión y Difusión Doctrinal
            </div>
            <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight mb-6">
                CANALES OFICIALES
            </h2>
            <p class="text-gray-300 text-sm sm:text-base max-w-2xl mx-auto mb-8">
                Acceda a las transmisiones, análisis tácticos y contenidos audibles oficiales del Codex Bellator a través de nuestras plataformas autorizadas:
            </p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-6">
                <!-- Canal de YouTube -->
                <a href="https://youtube.com/@cbau_oficial?si=kCZbinpbCuyRJNiU" 
                   target="_blank" 
                   rel="noopener noreferrer" 
                   class="w-full sm:w-auto px-6 py-4 bg-red-600 hover:bg-red-500 text-white font-bold uppercase tracking-wider text-sm rounded-xl transition-all shadow-lg flex items-center justify-center gap-3">
                    <i class="fa-brands fa-youtube text-xl"></i>
                    <span>Canal Oficial de YouTube</span>
                    <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i>
                </a>
                <!-- Canal de Spotify -->
                <a href="https://open.spotify.com/show/3TW9W430Awp2kJrsfyQmPD?si=jmxnEVngRR-X1-TL6p2yig&utm_source=copy-link" 
                   target="_blank" 
                   rel="noopener noreferrer" 
                   class="w-full sm:w-auto px-6 py-4 bg-emerald-600 hover:bg-emerald-500 text-white font-bold uppercase tracking-wider text-sm rounded-xl transition-all shadow-lg flex items-center justify-center gap-3">
                    <i class="fa-brands fa-spotify text-xl"></i>
                    <span>Canal Oficial de Spotify</span>
                    <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- SECCIÓN DE DESCARGA -->
    <section id="descarga" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/80 border-2 border-amber-500/80 rounded-2xl p-6 sm:p-10 shadow-2xl glow-amber text-center">
            <h2 class="text-2xl sm:text-4xl font-black text-white uppercase tracking-tight mb-4">
                CODEX BELLATOR — DOCUMENTO COMPLETO
            </h2>
            <p class="text-gray-300 text-sm sm:text-base mb-8 max-w-2xl mx-auto">
                Descargue o consulte el repositorio doctrinal completo en Google Drive para profundizar en cada protocolo técnico y matemático.
            </p>
            <a href="https://docs.google.com/document/d/1YEmlGMu-T34Esf-Be0_Mozz6hsiME5ww/edit?usp=drivesdk&ouid=115977733970390058232&rtpof=true&sd=true" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="inline-flex items-center gap-3 px-8 py-4 bg-amber-500 hover:bg-amber-400 text-black font-black uppercase tracking-wider text-sm rounded-xl transition-all shadow-xl">
                <i class="fa-solid fa-file-lines text-lg"></i>
                <span>📄 DESCARGAR CODEX COMPLETO EN GOOGLE DRIVE</span>
            </a>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-tactical-900 border-t border-tactical-800 py-8 text-center text-xs text-gray-500 font-mono">
        <div class="max-w-7xl mx-auto px-4 space-y-2">
            <p>© CODEX BELLATOR - ARS UNIFIED. Ciencia de Combate Unificado.</p>
            <p class="text-amber-500/70">Soberanía Neural • Inevitabilidad Táctica • Tiempo Cero (T0)</p>
        </div>
    </footer>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Menú móvil
            const menuBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            if (menuBtn && mobileMenu) {
                menuBtn.addEventListener('click', () => mobileMenu.classList.toggle('hidden'));
                mobileLinks.forEach(link => link.addEventListener('click', () => mobileMenu.classList.add('hidden')));
            }

            // Pestañas (Tabs)
            const tabButtons = document.querySelectorAll('.tab-btn');
            const tabPanes = document.querySelectorAll('.tab-pane');

            tabButtons.forEach(btn => {
                btn.addEventListener('click', () => {
                    const targetId = btn.getAttribute('data-target');
                    tabPanes.forEach(pane => pane.classList.add('hidden'));
                    tabButtons.forEach(b => {
                        b.classList.remove('bg-amber-500', 'text-black', 'shadow-md', 'active');
                        b.classList.add('bg-tactical-700', 'text-gray-300');
                    });
                    const targetPane = document.getElementById(targetId);
                    if (targetPane) targetPane.classList.remove('hidden');
                    btn.classList.remove('bg-tactical-700', 'text-gray-300');
                    btn.classList.add('bg-amber-500', 'text-black', 'shadow-md', 'active');
                });
            });

            // Simulador ST
            const inputSt = document.getElementById('input-st');
            const valSt = document.getElementById('val-st');
            const statusBox = document.getElementById('status-box');

            if (inputSt) {
                inputSt.addEventListener('input', (e) => {
                    const val = parseFloat(e.target.value);
                    valSt.innerText = val.toFixed(1);
                    if (val < 5.0) {
                        statusBox.className = "p-3 rounded-xl border mt-4 bg-red-500/20 border-red-500 text-red-300 text-center text-xs font-mono";
                        statusBox.innerText = "PROGRESIÓN BLOQUEADA: Voto de Censura Activo (ST < 5.0)";
                    } else {
                        statusBox.className = "p-3 rounded-xl border mt-4 bg-emerald-500/20 border-emerald-500 text-emerald-300 text-center text-xs font-mono";
                        statusBox.innerText = "PROGRESIÓN AUTORIZADA: Umbral superado (≥ 5.0)";
                    }
                });
            }
        });
    </script>
</body>
</html>
