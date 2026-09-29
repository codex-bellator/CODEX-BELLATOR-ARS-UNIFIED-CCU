<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
        .border-gradient {
            border-image: linear-gradient(to right, #f59e0b, #06b6d4) 1;
        }
        /* Custom scrollbar */
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
            <nav class="hidden lg:flex items-center gap-6 text-xs font-semibold tracking-wider uppercase text-gray-300">
                <a href="#que-es" class="hover:text-amber-400 transition-colors">¿Qué es?</a>
                <a href="#para-que-sirve" class="hover:text-amber-400 transition-colors">¿Para qué sirve?</a>
                <a href="#objetivo" class="hover:text-amber-400 transition-colors">Objetivo</a>
                <a href="#como-funciona" class="hover:text-amber-400 transition-colors">Funcionamiento</a>
                <a href="#realmente-funciona" class="hover:text-amber-400 transition-colors">Evidencia</a>
                <a href="#diferencias" class="hover:text-amber-400 transition-colors">Comparativa</a>
                <a href="#descarga" class="hover:text-amber-400 transition-colors text-amber-400">Descarga</a>
            </nav>

            <!-- Acceso Rápido a Redes y Botón de Explorar -->
            <div class="flex items-center gap-3">
                <div class="hidden sm:flex items-center gap-2 border-r border-tactical-700 pr-3">
                    <a href="https://youtube.com/@cbau_oficial?si=kCZbinpbCuyRJNiU" target="_blank" rel="noopener noreferrer" title="Canal Oficial de YouTube" class="p-2 text-gray-400 hover:text-red-500 transition-colors">
                        <i class="fa-brands fa-youtube text-lg"></i>
                    </a>
                    <a href="https://open.spotify.com/show/3TW9W430Awp2kJrsfyQmPD?si=jmxnEVngRR-X1-TL6p2yig&utm_source=copy-link" target="_blank" rel="noopener noreferrer" title="Canal Oficial de Spotify" class="p-2 text-gray-400 hover:text-green-500 transition-colors">
                        <i class="fa-brands fa-spotify text-lg"></i>
                    </a>
                </div>

                <a href="#conocer" class="px-4 py-2 text-xs font-bold uppercase tracking-wider bg-amber-500 text-black rounded-lg hover:bg-amber-400 transition-all shadow-lg shadow-amber-500/20 flex items-center gap-2">
                    <i class="fa-solid fa-book-bookmark"></i>
                    <span class="hidden sm:inline">Explorar Codex</span>
                </a>
                <button id="mobile-menu-btn" class="lg:hidden p-2 text-gray-400 hover:text-white">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile dropdown menu -->
        <div id="mobile-menu" class="hidden lg:hidden bg-tactical-800 border-b border-tactical-700 px-4 py-4 space-y-3 text-sm">
            <a href="#que-es" class="block text-gray-300 hover:text-amber-400 font-medium">¿Qué es el Codex?</a>
            <a href="#para-que-sirve" class="block text-gray-300 hover:text-amber-400 font-medium">¿Para qué sirve?</a>
            <a href="#objetivo" class="block text-gray-300 hover:text-amber-400 font-medium">¿Cuál es su objetivo?</a>
            <a href="#como-funciona" class="block text-gray-300 hover:text-amber-400 font-medium">¿Cómo funciona?</a>
            <a href="#realmente-funciona" class="block text-gray-300 hover:text-amber-400 font-medium">¿Realmente funciona?</a>
            <a href="#diferencias" class="block text-gray-300 hover:text-amber-400 font-medium">Diferencias Metodológicas</a>
            <a href="#descarga" class="block text-amber-400 hover:text-amber-300 font-bold">Descargar Codex Completo</a>
            
            <div class="pt-3 border-t border-tactical-700 flex items-center gap-4">
                <span class="text-xs text-gray-400 font-mono">Canales:</span>
                <a href="https://youtube.com/@cbau_oficial?si=kCZbinpbCuyRJNiU" target="_blank" class="text-red-500 hover:text-red-400 font-bold flex items-center gap-1 text-xs">
                    <i class="fa-brands fa-youtube"></i> YouTube
                </a>
                <a href="https://open.spotify.com/show/3TW9W430Awp2kJrsfyQmPD?si=jmxnEVngRR-X1-TL6p2yig&utm_source=copy-link" target="_blank" class="text-green-500 hover:text-green-400 font-bold flex items-center gap-1 text-xs">
                    <i class="fa-brands fa-spotify"></i> Spotify
                </a>
            </div>
        </div>
    </header>

    <!-- MAIN BLOGGER HERO BLOCK -->
    <section class="relative pt-12 pb-16 px-4 sm:px-6 lg:px-8 max-w-5xl mx-auto text-center" id="conocer">
        <div class="absolute inset-0 -z-10 bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-amber-500/10 via-tactical-900/60 to-transparent"></div>
        
        <!-- Hero Box Frame -->
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

            <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-8">
                <a href="#que-es" class="w-full sm:w-auto px-8 py-4 bg-amber-500 hover:bg-amber-400 text-black font-black uppercase tracking-widest text-sm rounded-xl transition-all shadow-xl hover:scale-105 flex items-center justify-center gap-3">
                    <span>[ CONOCER EL CODEX ]</span>
                    <i class="fa-solid fa-arrow-down"></i>
                </a>
                <a href="#descarga" class="w-full sm:w-auto px-6 py-4 bg-tactical-700 hover:bg-tactical-600 text-amber-400 font-bold uppercase tracking-wider text-sm rounded-xl transition-all border border-amber-500/30 flex items-center justify-center gap-2">
                    <i class="fa-solid fa-file-pdf"></i>
                    <span>Documento Completo</span>
                </a>
            </div>

            <!-- SECCIÓN NUEVA: CANALES OFICIALES DE DIFUSIÓN -->
            <div class="p-4 bg-tactical-900/90 rounded-xl border border-tactical-700 max-w-xl mx-auto">
                <span class="text-xs font-mono uppercase text-gray-400 tracking-widest block mb-3">
                    <i class="fa-solid fa-broadcast-tower text-amber-500 mr-1"></i> Canales Oficiales de Difusión
                </span>
                <div class="flex flex-col sm:flex-row items-center justify-center gap-3">
                    <a href="https://youtube.com/@cbau_oficial?si=kCZbinpbCuyRJNiU" target="_blank" rel="noopener noreferrer" class="w-full sm:w-1/2 px-4 py-2.5 bg-red-600/20 hover:bg-red-600/30 text-red-400 border border-red-500/40 rounded-lg text-xs font-bold uppercase tracking-wider transition-all flex items-center justify-center gap-2">
                        <i class="fa-brands fa-youtube text-lg text-red-500"></i>
                        <span>Canal de YouTube</span>
                    </a>
                    <a href="https://open.spotify.com/show/3TW9W430Awp2kJrsfyQmPD?si=jmxnEVngRR-X1-TL6p2yig&utm_source=copy-link" target="_blank" rel="noopener noreferrer" class="w-full sm:w-1/2 px-4 py-2.5 bg-green-600/20 hover:bg-green-600/30 text-green-400 border border-green-500/40 rounded-lg text-xs font-bold uppercase tracking-wider transition-all flex items-center justify-center gap-2">
                        <i class="fa-brands fa-spotify text-lg text-green-500"></i>
                        <span>Podcast Spotify</span>
                    </a>
                </div>
            </div>

            <div class="mt-8 pt-6 border-t border-tactical-700/80 flex flex-wrap justify-center gap-4 text-xs text-gray-400 font-mono">
                <span><i class="fa-solid fa-shield text-amber-500 mr-1"></i>Arquitectura Metodológica Canónica</span>
                <span>•</span>
                <span><i class="fa-solid fa-code-branch text-amber-500 mr-1"></i>Doctrina Versión 4.0 (Sistémica Avanzada)</span>
                <span>•</span>
                <span><i class="fa-solid fa-microchip text-amber-500 mr-1"></i>P.A.O. v6.0 & S.M.V.</span>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl animate-bounce">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 1: ¿QUÉ ES EL CODEX BELLATOR ARS UNIFIED? -->
    <section id="que-es" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    1
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿QUÉ ES EL CODEX BELLATOR ARS UNIFIED?
                </h2>
            </div>

            <div class="prose prose-invert max-w-none text-gray-300 text-base sm:text-lg leading-relaxed space-y-6">
                <p class="font-medium text-amber-200/90 text-lg sm:text-xl border-l-4 border-amber-500 pl-4 py-1">
                    El <strong>Codex Bellator – Ars Unified</strong> es la <strong>Ciencia de Combate Unificado (C.C.U.)</strong>: un sistema cerrado de alta ingeniería humana, neurofisiología aplicada, biomecánica y telemetría biológica concebido para eliminar la entropía metodológica y la improvisación en las artes marciales y deportes de contacto.
                </p>

                <p>
                    A diferencia del entrenamiento tradicional basado en la acumulación ciega de fatiga muscular y dogmas históricos, el Codex concibe el combate como un <strong>proceso dinámico de control de lazo cerrado</strong>. Su fin es transformar al atleta en un operador capaz de anular la latencia reactiva del oponente y ejecutar intercepciones en <strong>Tiempo Cero ($T0$)</strong>.
                </p>

                <!-- 3 Levels of Abstraction Grid -->
                <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-4 pt-4">
                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-amber-500/50 transition-colors">
                        <div class="text-amber-500 font-mono text-xs uppercase font-bold mb-1">Nivel 1 • Límite Constitucional</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-gavel text-amber-500 mr-2"></i>La Regla</h3>
                        <p class="text-xs text-gray-400">Establece el límite biomecánico e inmutable que garantiza la seguridad del chasis y la pureza del engrama motor del combatiente. Define el <em>"qué debe cumplirse"</em>.</p>
                    </div>

                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-cyan-500/50 transition-colors">
                        <div class="text-cyan-400 font-mono text-xs uppercase font-bold mb-1">Nivel 2 • Telemetría</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-table text-cyan-400 mr-2"></i>La Plantilla</h3>
                        <p class="text-xs text-gray-400">Receptáculo físico estructurado donde se registran metadatos y telemetría biológica del atleta, desterrando notas libres y subjetividades. Define el <em>"dónde se registra"</em>.</p>
                    </div>

                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-amber-500/50 transition-colors">
                        <div class="text-amber-500 font-mono text-xs uppercase font-bold mb-1">Nivel 3 • Hoja de Ruta Algorítmica</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-diagram-project text-amber-500 mr-2"></i>El P.A.O.</h3>
                        <p class="text-xs text-gray-400">Protocolo de Aplicación Operativa: guía procedimental paso a paso que instruye al operador sobre cómo rellenar plantillas y aplicar reglas sin sesgo. Define el <em>"cómo se procede"</em>.</p>
                    </div>
                </div>

                <!-- Principle of Flow Continuity callout -->
                <div class="bg-amber-500/10 border border-amber-500/30 rounded-xl p-5 mt-6">
                    <h4 class="text-amber-400 font-bold uppercase text-sm flex items-center gap-2 mb-2">
                        <i class="fa-solid fa-arrows-spin text-lg"></i>
                        Principio Rector Supremo: Regla de Continuidad de Flujo
                    </h4>
                    <p class="text-xs sm:text-sm text-gray-300">
                        La famosa expresión <code class="bg-tactical-900 px-2 py-0.5 rounded text-amber-300 font-mono">A+D+A = 1</code> constituye un modelo paradigmático de integración temporal y funcional (Ataque + Defensa + Continuidad sin bloques independientes), y <strong>NO una secuencia fija u obligatoria</strong>. En el Codex, toda retracción o transición de masa es la defensa activa y la precarga bioeléctrica del siguiente ataque, erradicando los tiempos muertos.
                    </p>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 2: ¿PARA QUÉ SIRVE? -->
    <section id="para-que-sirve" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    2
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿PARA QUÉ SIRVE?
                </h2>
            </div>

            <p class="text-gray-300 text-base sm:text-lg mb-8 leading-relaxed">
                El Codex Bellator sirve como una <strong>plataforma de soberanía y optimización biomecánica integral</strong>. Sus aplicaciones abarcan desde la preparación física de alta precisión hasta el combate real en todas las distancias.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Card 1 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-amber-500/40 transition-all flex gap-4">
                    <div class="text-amber-500 text-2xl shrink-0">
                        <i class="fa-solid fa-stopwatch-20"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Anulación de Latencia Reactiva (Tiempo Cero)</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Permite al peleador detectar las microseñales biomecánicas del oponente antes de que su golpe madure, disparando el vector de intercepción en la génesis ($FF1$) e invalidando el tiempo de respuesta convencional (~200ms).
                        </p>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-cyan-500/40 transition-all flex gap-4">
                    <div class="text-cyan-400 text-2xl shrink-0">
                        <i class="fa-solid fa-shield-virus"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Protección del Chasis y Prevención de Lesiones</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Mediante el <strong>Umbral de Velocidad Crítica (UVC 10%)</strong> y el protocolo de Chasis Seguro, aborta de forma automática las series cuando la velocidad cae, erradicando el "volumen basura" que degrada las articulaciones y corrompe el engrama.
                        </p>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-amber-500/40 transition-all flex gap-4">
                    <div class="text-amber-500 text-2xl shrink-0">
                        <i class="fa-solid fa-person-ripping"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Unificación Striking & Grappling / Suelo</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Aplica de manera idéntica en combate de pie y combate de agarre (Judo, Lucha, BJJ). Rige la presión gravitacional cohesiva ($PFM-2$) y las cuñas mecánicas ($PFM-3$) para neutralizar barridos y derribos sin perder la plomada.
                        </p>
                    </div>
                </div>

                <!-- Card 4 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-cyan-500/40 transition-all flex gap-4">
                    <div class="text-cyan-400 text-2xl shrink-0">
                        <i class="fa-solid fa-chart-line"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Auditoría Cuantitativa Transparente</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Proporciona a entrenadores y atletas indicadores matemáticos inexpugnables ($IGD$, $I.I.S.$, $I.P.F.$) para evaluar la frescura neural y tomar decisiones adaptativas con el algoritmo <strong>IA-P1</strong>.
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 3: ¿CUÁL ES SU OBJETIVO? -->
    <section id="objetivo" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl relative overflow-hidden">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    3
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿CUÁL ES SU OBJETIVO?
                </h2>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6 items-center">
                <div class="lg:col-span-2 space-y-4 text-gray-300 text-base leading-relaxed">
                    <p class="text-lg font-semibold text-white">
                        La finalidad suprema perseguida por la Ciencia de Combate Unificado es alcanzar la <span class="text-amber-400 underline decoration-amber-500/50">Soberanía Neural y la Inevitabilidad Táctica</span> en la contienda.
                    </p>
                    <p>
                        El objetivo no es simplemente ganar un asalto mediante desgaste aleatorio, sino <strong>dominar el espacio-tiempo de la pelea (Kairós)</strong>, erradicando la duda, la vacilación y los tiempos muertos a través de las 5 dimensiones del engrama motor subcortical (Estado de Integración $EI-5$).
                    </p>
                    <ul class="space-y-2 text-xs sm:text-sm font-mono text-gray-300 pt-2">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Desatar el reclutamiento voluntario instantáneo de Fibras Rápidas Tipo IIa y IIx.</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Reprogramar las respuestas reactivas para ser procesadas en el cerebelo en silencio cognitivo.</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Maximizar la rentabilidad biológica del entrenamiento mediante el Índice de Costo-Beneficio ($ICB$).</li>
                    </ul>
                </div>

                <!-- Goal Pillar Highlight Box -->
                <div class="bg-gradient-to-br from-amber-500/20 to-tactical-900 border border-amber-500/40 p-6 rounded-xl text-center glow-amber">
                    <i class="fa-solid fa-bullseye text-4xl text-amber-400 mb-3 block"></i>
                    <h3 class="font-black text-white text-lg uppercase tracking-wider mb-2">Meta Final</h3>
                    <p class="text-xs text-amber-200/80 leading-relaxed font-mono">
                        "Convertir la respuesta defensiva y ofensiva en una sola vibración cinemática indivisible en Tiempo Cero (Lin Sil Die Dar)."
                    </p>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 4: ¿CÓMO FUNCIONA? -->
    <section id="como-funciona" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    4
                </div>
                <div>
                    <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                        ¿CÓMO FUNCIONA?
                    </h2>
                    <p class="text-xs text-amber-400 font-mono uppercase">Estructura algorítmica y arquitectura de lazo cerrado</p>
                </div>
            </div>

            <!-- Principios Fundamentales -->
            <div class="bg-tactical-900/90 rounded-xl p-6 border border-tactical-700/80 space-y-4">
                <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                    <h3 class="text-base sm:text-lg font-bold text-cyan-400">Principios Fundamentales del Movimiento (P.F.M.)</h3>
                    <span class="text-[10px] sm:text-xs font-mono bg-cyan-500/20 text-cyan-300 px-2 py-1 rounded">Leyes Biomecánicas Inmutables</span>
                </div>
                <p class="text-xs sm:text-sm leading-relaxed text-gray-300">
                    Las leyes físicas rectoras que gobiernan la geometría corporal tanto en Golpeo (Striking) como en Agarre/Suelo (Grappling/Lucha/BJJ):
                </p>
                <div class="space-y-3 pt-2">
                    <div class="p-4 bg-tactical-800 rounded-lg border border-tactical-700">
                        <div class="text-amber-400 font-bold text-xs sm:text-sm font-mono">PFM-1: Eje Estructural</div>
                        <p class="text-xs sm:text-sm leading-relaxed text-gray-300 mt-1">Mantenimiento de la plomada vertical (cabeza-columna-cadera). En lucha/suelo opera como el pivote soberano que impide el colapso del centro de gravedad.</p>
                    </div>
                    <div class="p-4 bg-tactical-800 rounded-lg border border-tactical-700">
                        <div class="text-amber-400 font-bold text-xs sm:text-sm font-mono">PFM-2: Transferencia de Masa Cohesiva</div>
                        <p class="text-xs sm:text-sm leading-relaxed text-gray-300 mt-1">Inercia unificada del chasis. En el tapiz se transmutación en presión gravitacional sin espacios intersticiales sobre el oponente.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER DE CIERRE -->
    <footer class="border-t border-tactical-800 bg-tactical-900/95 py-8 mt-12">
        <div class="max-w-7xl mx-auto px-4 text-center space-y-4">
            <div class="flex justify-center items-center gap-6 text-xl">
                <a href="https://youtube.com/@cbau_oficial?si=kCZbinpbCuyRJNiU" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-red-500 transition-colors">
                    <i class="fa-brands fa-youtube"></i>
                </a>
                <a href="https://open.spotify.com/show/3TW9W430Awp2kJrsfyQmPD?si=jmxnEVngRR-X1-TL6p2yig&utm_source=copy-link" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-green-500 transition-colors">
                    <i class="fa-brands fa-spotify"></i>
                </a>
            </div>
            <p class="text-xs text-gray-500 font-mono">
                CODEX BELLATOR - ARS UNIFIED &copy; Ciencia de Combate Unificado. Todos los derechos reservados.
            </p>
        </div>
    </footer>

    <!-- Script opcional para menú móvil -->
    <script>
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');
        if (btn && menu) {
            btn.addEventListener('click', () => {
                menu.classList.toggle('hidden');
            });
        }
    </script>
</body>
</html>
