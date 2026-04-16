# FSallinone.ai
FS ALL IN ONE AI
ai-app/
├── backend/                    # Node.js/Express server
│   ├── routes/                 # API endpoints
│   ├── controllers/            # Business logic
│   ├── middleware/             # Auth, validation
│   ├── services/               # AI integrations
│   ├── models/                 # Database schemas
│   └── config/                 # Environment setup
├── frontend/                   # React/Vue UI
│   ├── components/             # Reusable UI
│   ├── pages/                  # Routes
│   ├── services/               # API calls
│   └── styles/                 # CSS/Tailwind
├── database/                   # SQLite/PostgreSQL
├── docker-compose.yml          # Local dev setup
├── .env.example                # Config template
└── README.md                   # Documentation
<html lang="en"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FSallinone.ai - Workspace</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://code.iconify.design/iconify-icon/1.0.7/iconify-icon.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500&amp;family=JetBrains+Mono:wght@400;500&amp;display=swap" rel="stylesheet">
</head>
<body class="bg-black text-zinc-300 antialiased selection:bg-purple-500/30 min-h-screen flex flex-col font-sans relative" style="font-family: 'Inter', sans-serif;">

    <!-- Subtle IDE-like Background Grid -->
    <div class="fixed inset-0 z-[-1] bg-[linear-gradient(to_right,#27272a33_1px,transparent_1px),linear-gradient(to_bottom,#27272a33_1px,transparent_1px)] bg-[size:1.5rem_1.5rem]"></div>
    <!-- Caffeine-like Ambient Glow -->
    <div class="fixed top-0 left-1/2 -translate-x-1/2 w-[40rem] h-[30rem] bg-gradient-to-b from-purple-900/20 via-blue-900/10 to-transparent blur-[100px] pointer-events-none -z-10"></div>

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 w-full border-b border-zinc-800 bg-black/80 backdrop-blur-md">
        <div class="max-w-[90rem] mx-auto px-4 sm:px-6 lg:px-8 h-14 flex items-center justify-between">
            <!-- Custom Logo Configuration -->
            <div class="flex items-center gap-4">
                <div class="relative flex flex-col items-center justify-center w-10 h-10 select-none">
                    <span class="absolute text-3xl font-medium text-zinc-800/80 tracking-tight z-0">FS</span>
                    <span class="relative text-xl font-medium bg-clip-text text-transparent bg-gradient-to-r from-red-500 via-purple-500 to-blue-500 z-10 tracking-tight">AI</span>
                </div>
                <div class="h-4 w-px bg-zinc-800 hidden sm:block"></div>
                <span class="text-sm font-medium text-zinc-400 hidden sm:block font-mono" style="font-family: 'JetBrains Mono', monospace;">workspace_main</span>
            </div>

            <!-- Auth & Credits -->
            <div class="flex items-center gap-4">
                <div class="hidden md:flex items-center gap-2 px-3 py-1 bg-zinc-900/80 border border-zinc-800 rounded-md text-xs font-mono text-zinc-300 shadow-[0_0_10px_rgba(168,85,247,0.1)]" style="font-family: 'JetBrains Mono', monospace;">
                    <iconify-icon icon="solar:bolt-linear" class="text-purple-500 text-sm" style="stroke-width: 1.5;"></iconify-icon>
                    <span>1,000_credits</span>
                </div>
                
                <button class="text-sm font-normal text-zinc-400 hover:text-white transition-colors duration-200 hidden sm:block">Log in</button>
                <a href="#signup" class="group relative inline-flex items-center justify-center px-4 py-1.5 text-sm font-medium text-white transition-all duration-200 bg-white text-black rounded-md hover:bg-zinc-200">
                    Run Workspace
                </a>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="flex-grow max-w-[90rem] w-full mx-auto p-4 sm:p-6 lg:p-8 flex flex-col gap-8">
        
        <!-- Hero Section (Replit IDE Window Style) -->
        <section class="relative rounded-xl border border-zinc-800 bg-black overflow-hidden shadow-[0_0_40px_-15px_rgba(168,85,247,0.2)]">
            <!-- Mac/IDE Window Header -->
            <div class="h-10 border-b border-zinc-800 bg-zinc-900/50 flex items-center justify-between px-4">
                <div class="flex items-center gap-2">
                    <div class="w-3 h-3 rounded-full bg-red-500/80 border border-red-500"></div>
                    <div class="w-3 h-3 rounded-full bg-purple-500/80 border border-purple-500"></div>
                    <div class="w-3 h-3 rounded-full bg-blue-500/80 border border-blue-500"></div>
                </div>
                <div class="text-xs text-zinc-500 font-mono" style="font-family: 'JetBrains Mono', monospace;">fs_all_in_one.sh</div>
                <div class="w-16"></div> <!-- Spacer for balance -->
            </div>

            <!-- IDE Body -->
            <div class="flex flex-col md:flex-row relative">
                <!-- Sidebar -->
                <div class="hidden md:flex flex-col w-64 border-r border-zinc-800 bg-black/50 p-4 shrink-0">
                    <span class="text-xs font-mono text-zinc-500 mb-4 uppercase tracking-widest" style="font-family: 'JetBrains Mono', monospace;">Explorer</span>
                    <ul class="space-y-2 text-sm font-medium text-zinc-400">
                        <li class="flex items-center gap-2 text-white bg-zinc-900/80 px-2 py-1.5 rounded-md border border-zinc-800">
                            <iconify-icon icon="solar:folder-with-files-linear" class="text-blue-400"></iconify-icon>
                            app_builder
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:monitor-smartphone-linear" class="text-purple-400"></iconify-icon>
                            web_generator
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:gallery-edit-linear" class="text-red-400"></iconify-icon>
                            ad_studio
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:user-circle-linear" class="text-blue-400"></iconify-icon>
                            face_engine
                        </li>
                    </ul>
                </div>

                <!-- Main Editor Area -->
                <div class="flex-grow p-6 md:p-12 lg:p-20 relative overflow-hidden">
                    <!-- Subtle gradient behind text -->
                    <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-3/4 h-3/4 bg-gradient-to-tr from-red-600/10 via-purple-600/10 to-blue-600/10 blur-3xl rounded-full pointer-events-none"></div>
                    
                    <div class="relative z-10 max-w-3xl">
                        <div class="inline-flex items-center gap-2 px-3 py-1 mb-6 rounded-md border border-zinc-800 bg-zinc-950 text-xs font-mono text-zinc-400" style="font-family: 'JetBrains Mono', monospace;">
                            <span class="text-purple-500">&gt;</span> system initialized. 1000 credits granted.
                        </div>
                        <h1 class="text-4xl md:text-5xl font-medium text-white tracking-tight leading-tight mb-6">
                            Do anything. <span class="text-zinc-500">Build everything.</span> <br>
                            <span class="bg-clip-text text-transparent bg-gradient-to-r from-red-400 via-purple-400 to-blue-400 tracking-tight">All in one workspace.</span>
                        </h1>
                        <p class="text-base md:text-lg text-zinc-400 mb-10 font-light leading-relaxed max-w-xl">
                            Create apps, generate websites, turn photos into stunning ads, and swap faces instantly. Run the engine, spend credits, and deploy.
                        </p>
                        <div class="flex flex-col sm:flex-row items-center gap-4">
                            <a href="#signup" class="w-full sm:w-auto px-6 py-2.5 rounded-md bg-white text-black font-medium text-sm hover:bg-zinc-200 transition-colors flex items-center justify-center gap-2">
                                <iconify-icon icon="solar:play-circle-linear" style="stroke-width: 1.5;" class="text-lg"></iconify-icon>
                                Initialize Account
                            </a>
                            <a href="#pro" class="w-full sm:w-auto px-6 py-2.5 rounded-md bg-black text-white font-medium text-sm border border-zinc-800 hover:border-zinc-600 transition-colors flex items-center justify-center gap-2">
                                <iconify-icon icon="solar:crown-star-linear" style="stroke-width: 1.5;" class="text-purple-400 text-lg"></iconify-icon>
                                View Pro Config
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Features Grid (Terminal Card Style) -->
        <section class="py-12">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-8">
                <div>
                    <h2 class="text-2xl md:text-3xl font-medium text-white tracking-tight mb-2">Creative Modules</h2>
                    <p class="text-sm font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">cost: 10_credits / execution</p>
                </div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                
                <!-- Feature 1 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-blue-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-blue-500"></iconify-icon> app_builder.tsx</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-blue-500/5 blur-3xl group-hover:bg-blue-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">AI App Builder</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Describe your idea and watch our AI code, design, and deploy a fully functional mobile application in minutes.</p>
                        <button class="self-start text-xs font-mono text-blue-400 hover:text-blue-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 2 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-purple-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-purple-500"></iconify-icon> web_gen.html</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-purple-500/5 blur-3xl group-hover:bg-purple-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Website Generator</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Build stunning, responsive websites. Just provide a prompt, and get a complete site ready for the web.</p>
                        <button class="self-start text-xs font-mono text-purple-400 hover:text-purple-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 3 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-red-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-red-500"></iconify-icon> ad_studio.psd</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-red-500/5 blur-3xl group-hover:bg-red-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Ad Studio &amp; Editor</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Select photos from your gallery, apply AI filters, and instantly generate high-converting advertisement graphics.</p>
                        <button class="self-start text-xs font-mono text-red-400 hover:text-red-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 4 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-blue-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-blue-400"></iconify-icon> face_engine.py</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-blue-400/5 blur-3xl group-hover:bg-blue-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Face AI Studio</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Advanced facial manipulation. Change faces, adjust expressions, or create entirely new hyper-realistic personas.</p>
                        <button class="self-start text-xs font-mono text-blue-400 hover:text-blue-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 5 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-purple-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-purple-400"></iconify-icon> omni_core.rs</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-purple-400/5 blur-3xl group-hover:bg-purple-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Omnipotent AI</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Text, voice, code, or data analysis—whatever you want to do, our core AI engine is equipped to handle it.</p>
                        <button class="self-start text-xs font-mono text-purple-400 hover:text-purple-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 6 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-red-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-red-400"></iconify-icon> video_studio.mp4</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-red-400/5 blur-3xl group-hover:bg-red-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">AI Video Studio</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Turn text prompts or static images into dynamic, high-quality video sequences instantly.</p>
                        <button class="self-start text-xs font-mono text-red-400 hover:text-red-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

            </div>
        </section>

        <!-- Pro Version Section (Caffeine Glow Vibe) -->
        <section id="pro" class="py-12 relative">
            <div class="absolute inset-0 bg-gradient-to-r from-red-500/5 via-purple-500/5 to-blue-500/5 rounded-3xl blur-2xl pointer-events-none"></div>
            
            <div class="relative rounded-2xl border border-zinc-800 bg-black overflow-hidden">
                <!-- Top glowing border effect -->
                <div class="absolute top-0 left-0 right-0 h-px bg-gradient-to-r from-red-500 via-purple-500 to-blue-500 opacity-50"></div>
                
                <div class="p-8 md:p-12 flex flex-col md:flex-row items-center justify-between gap-10">
                    <div class="flex-1">
                        <div class="inline-flex items-center gap-2 px-3 py-1 mb-6 rounded-md bg-zinc-900 border border-zinc-800 text-xs font-mono text-zinc-300" style="font-family: 'JetBrains Mono', monospace;">
                            <span class="w-2 h-2 rounded-full bg-purple-500 animate-pulse"></span>
                            pro_environment_ready
                        </div>
                        <h2 class="text-3xl md:text-4xl font-medium text-white tracking-tight mb-4">Unlock ultimate freedom.</h2>
                        <ul class="space-y-4 mb-6 font-mono text-xs md:text-sm" style="font-family: 'JetBrains Mono', monospace;">
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.watermarks = false;</span> // Remove branding from outputs</span>
                            </li>
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.credits = 50000;</span> // Massive monthly allowance</span>
                            </li>
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.priority = "high";</span> // Skip queue with fast GPU processing</span>
                            </li>
                        </ul>
                    </div>
                    
                    <div class="w-full md:w-80 bg-zinc-900/50 border border-zinc-800 rounded-xl p-6 flex flex-col items-center text-center relative overflow-hidden group">
                        <div class="absolute inset-0 bg-gradient-to-br from-red-500/10 via-purple-500/10 to-blue-500/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                        <span class="text-xs font-mono text-zinc-500 mb-2" style="font-family: 'JetBrains Mono', monospace;">subscription.price</span>
                        <div class="flex items-baseline gap-1 mb-6">
                            <span class="text-4xl font-medium tracking-tight text-white">$19</span>
                            <span class="text-sm font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">/mo</span>
                        </div>
                        <button class="relative w-full py-2.5 rounded-md bg-white text-black font-medium text-sm hover:bg-zinc-200 transition-colors mb-3 overflow-hidden">
                            <span class="relative z-10">Upgrade to Pro</span>
                        </button>
                        <p class="text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">cancel_anytime == true</p>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-zinc-800 mt-auto bg-black relative z-10">
        <div class="max-w-[90rem] mx-auto px-4 sm:px-6 lg:px-8 py-6 flex flex-col md:flex-row items-center justify-between gap-4">
            <div class="flex items-center gap-3 select-none">
                 <div class="relative flex flex-col items-center justify-center w-6 h-6">
                    <span class="absolute text-xl font-medium text-zinc-800 tracking-tight z-0">FS</span>
                    <span class="relative text-xs font-medium bg-clip-text text-transparent bg-gradient-to-r from-red-500 via-purple-500 to-blue-500 z-10 tracking-tight">AI</span>
                </div>
                <span class="text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">©_2024_fsallinone.ai</span>
            </div>
            <div class="flex items-center gap-6 text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">
                <a href="#" class="hover:text-zinc-300 transition-colors">privacy.md</a>
                <a href="#" class="hover:text-zinc-300 transition-colors">terms.md</a>
                <a href="#" class="hover:text-zinc-300 transition-colors">support()</a>
            </div>
        </div>
    </footer>


</body></html>
<html lang="en"><head><meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FSallinone.ai - Workspace</title>
<!-- PWA & Installation Meta Tags -->
<meta name="application-name" content="FS.AI">
<meta name="apple-mobile-web-app-title" content="FS.AI">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="theme-color" content="#000000">
<link rel="manifest" href="data:application/manifest+json,{&quot;name&quot;:&quot;FSallinone.ai&quot;,&quot;short_name&quot;:&quot;FS.AI&quot;,&quot;start_url&quot;:&quot;.&quot;,&quot;display&quot;:&quot;standalone&quot;,&quot;background_color&quot;:&quot;#000000&quot;,&quot;theme_color&quot;:&quot;#000000&quot;}">

<script src="https://cdn.tailwindcss.com"></script>
<script src="https://code.iconify.design/iconify-icon/1.0.7/iconify-icon.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&amp;family=JetBrains+Mono:wght@400;500&amp;display=swap" rel="stylesheet"></head>
<body class="bg-black text-zinc-300 antialiased selection:bg-purple-500/30 min-h-screen flex flex-col font-sans relative" style="font-family: 'Inter', sans-serif;">

    <!-- Subtle IDE-like Background Grid -->
    <div class="fixed inset-0 z-[-1] bg-[linear-gradient(to_right,#27272a33_1px,transparent_1px),linear-gradient(to_bottom,#27272a33_1px,transparent_1px)] bg-[size:1.5rem_1.5rem]"></div>
    <!-- Ambient Glow -->
    <div class="fixed top-0 left-1/2 -translate-x-1/2 w-[40rem] h-[30rem] bg-gradient-to-b from-purple-900/20 via-blue-900/10 to-transparent blur-[100px] pointer-events-none -z-10"></div>

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 w-full border-b border-zinc-800 bg-black/80 backdrop-blur-md">
        <div class="max-w-[90rem] mx-auto px-4 sm:px-6 lg:px-8 h-14 flex items-center justify-between">
            <!-- Logo Configuration -->
            <div class="flex items-center gap-4">
                <a href="#" class="flex items-center gap-2.5 group">
                    <div class="relative flex items-center justify-center w-8 h-8 rounded-lg bg-gradient-to-tr from-red-500 via-purple-500 to-blue-500 shadow-lg shadow-purple-500/20 group-hover:shadow-purple-500/40 transition-all duration-300">
                        <div class="absolute inset-0 bg-black/20 rounded-lg backdrop-blur-sm border border-white/20"></div>
                        <iconify-icon icon="solar:infinity-linear" class="text-white text-xl relative z-10" style="stroke-width: 1.5;"></iconify-icon>
                    </div>
                    <span class="text-lg font-semibold text-white tracking-tight flex items-center">
                        FS<span class="text-transparent bg-clip-text bg-gradient-to-r from-red-400 via-purple-400 to-blue-400">.AI</span>
                    </span>
                </a>
                
                <div class="h-4 w-px bg-zinc-800 hidden sm:block"></div>
                <div class="hidden sm:flex items-center gap-2">
                    <span class="flex items-center gap-1.5 text-xs font-mono text-zinc-400 bg-zinc-900/80 border border-zinc-800 px-2 py-0.5 rounded-md" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="w-1.5 h-1.5 rounded-full bg-green-500 animate-pulse"></span>
                        live_public
                    </span>
                </div>
            </div>

            <!-- Auth & Credits -->
            <div class="flex items-center gap-4">
                
                <!-- Install App Button added here -->
                <button class="hidden sm:flex items-center gap-1.5 px-3 py-1.5 text-xs font-medium text-blue-400 bg-blue-500/10 border border-blue-500/20 rounded-md hover:bg-blue-500/20 transition-all duration-200">
                    <iconify-icon icon="solar:download-square-linear" style="stroke-width: 1.5;" class="text-sm"></iconify-icon>
                    Install App
                </button>

                <div class="hidden md:flex items-center gap-2 px-3 py-1.5 bg-zinc-900/80 border border-zinc-800 rounded-md text-xs font-mono text-zinc-300 shadow-[0_0_10px_rgba(168,85,247,0.1)]" style="font-family: 'JetBrains Mono', monospace;">
                    <iconify-icon icon="solar:bolt-linear" class="text-purple-500 text-sm" style="stroke-width: 1.5;"></iconify-icon>
                    <span>1,000_credits</span>
                </div>
                
                <button class="text-sm font-normal text-zinc-400 hover:text-white transition-colors duration-200 hidden sm:block">Log in</button>
                <a href="#signup" class="group relative inline-flex items-center justify-center px-4 py-1.5 text-sm font-medium text-white transition-all duration-200 bg-white text-black rounded-md hover:bg-zinc-200">
                    Run Workspace
                </a>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="flex-grow max-w-[90rem] w-full mx-auto p-4 sm:p-6 lg:p-8 flex flex-col gap-8">
        
        <!-- Hero Section (Replit IDE Window Style) -->
        <section class="relative rounded-xl border border-zinc-800 bg-black overflow-hidden shadow-[0_0_40px_-15px_rgba(168,85,247,0.2)]">
            <!-- Mac/IDE Window Header -->
            <div class="h-10 border-b border-zinc-800 bg-zinc-900/50 flex items-center justify-between px-4">
                <div class="flex items-center gap-2">
                    <div class="w-3 h-3 rounded-full bg-red-500/80 border border-red-500"></div>
                    <div class="w-3 h-3 rounded-full bg-purple-500/80 border border-purple-500"></div>
                    <div class="w-3 h-3 rounded-full bg-blue-500/80 border border-blue-500"></div>
                </div>
                <div class="text-xs text-zinc-500 font-mono" style="font-family: 'JetBrains Mono', monospace;">fs_all_in_one.sh</div>
                <div class="w-16"></div>
            </div>

            <!-- IDE Body -->
            <div class="flex flex-col md:flex-row relative">
                <!-- Sidebar -->
                <div class="hidden md:flex flex-col w-64 border-r border-zinc-800 bg-black/50 p-4 shrink-0">
                    <span class="text-xs font-mono text-zinc-500 mb-4 uppercase tracking-widest" style="font-family: 'JetBrains Mono', monospace;">Explorer</span>
                    <ul class="space-y-2 text-sm font-medium text-zinc-400">
                        <li class="flex items-center gap-2 text-white bg-zinc-900/80 px-2 py-1.5 rounded-md border border-zinc-800">
                            <iconify-icon icon="solar:folder-with-files-linear" class="text-blue-400"></iconify-icon>
                            app_builder
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:monitor-smartphone-linear" class="text-purple-400"></iconify-icon>
                            web_generator
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:gallery-edit-linear" class="text-red-400"></iconify-icon>
                            ad_studio
                        </li>
                        <li class="flex items-center gap-2 px-2 py-1.5 hover:text-white cursor-pointer transition-colors">
                            <iconify-icon icon="solar:user-circle-linear" class="text-blue-400"></iconify-icon>
                            face_engine
                        </li>
                    </ul>
                </div>

                <!-- Main Editor Area -->
                <div class="flex-grow p-6 md:p-12 lg:p-20 relative overflow-hidden">
                    <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-3/4 h-3/4 bg-gradient-to-tr from-red-600/10 via-purple-600/10 to-blue-600/10 blur-3xl rounded-full pointer-events-none"></div>
                    
                    <div class="relative z-10 max-w-3xl">
                        <div class="inline-flex items-center gap-2 px-3 py-1 mb-6 rounded-md border border-zinc-800 bg-zinc-950 text-xs font-mono text-zinc-400" style="font-family: 'JetBrains Mono', monospace;">
                            <span class="text-purple-500">&gt;</span> system initialized. 1000 credits granted.
                        </div>
                        <h1 class="text-4xl md:text-5xl font-medium text-white tracking-tight leading-tight mb-6">
                            Do anything. <span class="text-zinc-500">Build everything.</span> <br>
                            <span class="bg-clip-text text-transparent bg-gradient-to-r from-red-400 via-purple-400 to-blue-400 tracking-tight">All in one workspace.</span>
                        </h1>
                        <p class="text-base md:text-lg text-zinc-400 mb-10 font-light leading-relaxed max-w-xl">
                            Create apps, generate websites, turn photos into stunning ads, and swap faces instantly. Run the engine, spend credits, and deploy.
                        </p>
                        <div class="flex flex-col sm:flex-row items-center gap-4">
                            <a href="#signup" class="w-full sm:w-auto px-6 py-2.5 rounded-md bg-white text-black font-medium text-sm hover:bg-zinc-200 transition-colors flex items-center justify-center gap-2">
                                <iconify-icon icon="solar:play-circle-linear" style="stroke-width: 1.5;" class="text-lg"></iconify-icon>
                                Initialize Account
                            </a>
                            <a href="#pro" class="w-full sm:w-auto px-6 py-2.5 rounded-md bg-black text-white font-medium text-sm border border-zinc-800 hover:border-zinc-600 transition-colors flex items-center justify-center gap-2">
                                <iconify-icon icon="solar:crown-star-linear" style="stroke-width: 1.5;" class="text-purple-400 text-lg"></iconify-icon>
                                View Pro Config
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Features Grid (Terminal Card Style) -->
        <section class="py-12">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-8">
                <div>
                    <h2 class="text-2xl md:text-3xl font-medium text-white tracking-tight mb-2">Creative Modules</h2>
                    <p class="text-sm font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">cost: 10_credits / execution</p>
                </div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                
                <!-- Feature 1 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-blue-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-blue-500"></iconify-icon> app_builder.tsx</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-blue-500/5 blur-3xl group-hover:bg-blue-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">AI App Builder</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Describe your idea and watch our AI code, design, and deploy a fully functional mobile application in minutes.</p>
                        <button class="self-start text-xs font-mono text-blue-400 hover:text-blue-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 2 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-purple-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-purple-500"></iconify-icon> web_gen.html</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-purple-500/5 blur-3xl group-hover:bg-purple-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Website Generator</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Build stunning, responsive websites. Just provide a prompt, and get a complete site ready for the web.</p>
                        <button class="self-start text-xs font-mono text-purple-400 hover:text-purple-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 3 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-red-500/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-red-500"></iconify-icon> ad_studio.psd</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-red-500/5 blur-3xl group-hover:bg-red-500/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Ad Studio &amp; Editor</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Select photos from your gallery, apply AI filters, and instantly generate high-converting advertisement graphics.</p>
                        <button class="self-start text-xs font-mono text-red-400 hover:text-red-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 4 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-blue-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-blue-400"></iconify-icon> face_engine.py</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-blue-400/5 blur-3xl group-hover:bg-blue-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Face AI Studio</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Advanced facial manipulation. Change faces, adjust expressions, or create entirely new hyper-realistic personas.</p>
                        <button class="self-start text-xs font-mono text-blue-400 hover:text-blue-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 5 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-purple-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-purple-400"></iconify-icon> omni_core.rs</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-purple-400/5 blur-3xl group-hover:bg-purple-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">Omnipotent AI</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Text, voice, code, or data analysis—whatever you want to do, our core AI engine is equipped to handle it.</p>
                        <button class="self-start text-xs font-mono text-purple-400 hover:text-purple-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

                <!-- Feature 6 -->
                <div class="group relative rounded-xl bg-black border border-zinc-800 hover:border-red-400/50 transition-all duration-300 overflow-hidden flex flex-col">
                    <div class="border-b border-zinc-800/50 bg-zinc-900/50 px-4 py-2 flex items-center justify-between text-xs font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">
                        <span class="flex items-center gap-2"><iconify-icon icon="solar:code-linear" class="text-red-400"></iconify-icon> video_studio.mp4</span>
                        <span class="text-zinc-600">10c</span>
                    </div>
                    <div class="p-6 flex flex-col flex-grow relative">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-red-400/5 blur-3xl group-hover:bg-red-400/10 transition-colors rounded-full"></div>
                        <h3 class="text-lg font-medium text-white tracking-tight mb-2">AI Video Studio</h3>
                        <p class="text-sm text-zinc-400 leading-relaxed mb-4 flex-grow">Turn text prompts or static images into dynamic, high-quality video sequences instantly.</p>
                        <button class="self-start text-xs font-mono text-red-400 hover:text-red-300 flex items-center gap-1 transition-colors" style="font-family: 'JetBrains Mono', monospace;">
                            run_module() <iconify-icon icon="solar:arrow-right-linear"></iconify-icon>
                        </button>
                    </div>
                </div>

            </div>
        </section>

        <!-- Pro Version Section -->
        <section id="pro" class="py-12 relative">
            <div class="absolute inset-0 bg-gradient-to-r from-red-500/5 via-purple-500/5 to-blue-500/5 rounded-3xl blur-2xl pointer-events-none"></div>
            
            <div class="relative rounded-2xl border border-zinc-800 bg-black overflow-hidden">
                <!-- Top glowing border effect -->
                <div class="absolute top-0 left-0 right-0 h-px bg-gradient-to-r from-red-500 via-purple-500 to-blue-500 opacity-50"></div>
                
                <div class="p-8 md:p-12 flex flex-col md:flex-row items-center justify-between gap-10">
                    <div class="flex-1">
                        <div class="inline-flex items-center gap-2 px-3 py-1 mb-6 rounded-md bg-zinc-900 border border-zinc-800 text-xs font-mono text-zinc-300" style="font-family: 'JetBrains Mono', monospace;">
                            <span class="w-2 h-2 rounded-full bg-purple-500 animate-pulse"></span>
                            pro_environment_ready
                        </div>
                        <h2 class="text-3xl md:text-4xl font-medium text-white tracking-tight mb-4">Unlock ultimate freedom.</h2>
                        <ul class="space-y-4 mb-6 font-mono text-xs md:text-sm" style="font-family: 'JetBrains Mono', monospace;">
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.watermarks = false;</span> // Remove branding from outputs</span>
                            </li>
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.credits = 50000;</span> // Massive monthly allowance</span>
                            </li>
                            <li class="flex items-start gap-3 text-zinc-400">
                                <span class="text-green-500">✓</span>
                                <span><span class="text-zinc-200">env.priority = "high";</span> // Skip queue with fast GPU processing</span>
                            </li>
                        </ul>
                    </div>
                    
                    <div class="w-full md:w-80 bg-zinc-900/50 border border-zinc-800 rounded-xl p-6 flex flex-col items-center text-center relative overflow-hidden group">
                        <div class="absolute inset-0 bg-gradient-to-br from-red-500/10 via-purple-500/10 to-blue-500/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                        <span class="text-xs font-mono text-zinc-500 mb-2" style="font-family: 'JetBrains Mono', monospace;">subscription.price</span>
                        <div class="flex items-baseline gap-1 mb-6">
                            <span class="text-4xl font-medium tracking-tight text-white">$19</span>
                            <span class="text-sm font-mono text-zinc-500" style="font-family: 'JetBrains Mono', monospace;">/mo</span>
                        </div>
                        <button class="relative w-full py-2.5 rounded-md bg-white text-black font-medium text-sm hover:bg-zinc-200 transition-colors mb-3 overflow-hidden">
                            <span class="relative z-10">Upgrade to Pro</span>
                        </button>
                        <p class="text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">cancel_anytime == true</p>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-zinc-800 mt-auto bg-black relative z-10">
        <div class="max-w-[90rem] mx-auto px-4 sm:px-6 lg:px-8 py-6 flex flex-col md:flex-row items-center justify-between gap-4">
            
            <div class="flex items-center gap-4 select-none">
                <a href="#" class="flex items-center gap-2 group opacity-80 hover:opacity-100 transition-opacity">
                    <div class="relative flex items-center justify-center w-6 h-6 rounded-md bg-gradient-to-tr from-red-500 via-purple-500 to-blue-500">
                        <div class="absolute inset-0 bg-black/20 rounded-md border border-white/20"></div>
                        <iconify-icon icon="solar:infinity-linear" class="text-white text-xs relative z-10" style="stroke-width: 1.5;"></iconify-icon>
                    </div>
                    <span class="text-sm font-semibold text-white tracking-tight">
                        FS<span class="text-transparent bg-clip-text bg-gradient-to-r from-red-400 via-purple-400 to-blue-400">.AI</span>
                    </span>
                </a>
                <span class="text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">©_2024_published</span>
            </div>

            <div class="flex items-center gap-6 text-xs font-mono text-zinc-600" style="font-family: 'JetBrains Mono', monospace;">
                <a href="#" class="hover:text-zinc-300 transition-colors">privacy.md</a>
                <a href="#" class="hover:text-zinc-300 transition-colors">terms.md</a>
                <a href="#" class="hover:text-zinc-300 transition-colors">support()</a>
            </div>
        </div>
    </footer>

</body></html>
