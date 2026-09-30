
<!DOCTYPE html>
<html lang="en" class="scroll-smooth dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex Rivera | Senior Social Media Strategist & Brand Architect</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            purple: '#8B5CF6',
                            pink: '#EC4899',
                            cyan: '#06B6D4',
                            dark: '#0F172A',
                            card: '#1E293B',
                            lightCard: '#334155'
                        }
                    },
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'Inter', 'sans-serif'],
                    },
                    animation: {
                        'gradient-x': 'gradient-x 15s ease infinite',
                        'float': 'float 6s ease-in-out infinite',
                        'pulse-glow': 'pulse-glow 3s infinite',
                        'ticker': 'ticker 25s linear infinite',
                    },
                    keyframes: {
                        'gradient-x': {
                            '0%, 100%': { 'background-size': '200% 200%', 'background-position': 'left center' },
                            '50%': { 'background-size': '200% 200%', 'background-position': 'right center' },
                        },
                        'float': {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-12px)' },
                        },
                        'pulse-glow': {
                            '0%, 100%': { opacity: '0.4', filter: 'blur(20px)' },
                            '50%': { opacity: '0.8', filter: 'blur(30px)' },
                        },
                        'ticker': {
                            '0%': { transform: 'translateX(0%)' },
                            '100%': { transform: 'translateX(-50%)' }
                        }
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; }
        .glass-card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .text-gradient {
            background: linear-gradient(135deg, #EC4899 0%, #8B5CF6 50%, #06B6D4 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .bg-gradient-brand {
            background: linear-gradient(135deg, #EC4899 0%, #8B5CF6 50%, #06B6D4 100%);
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #0F172A; }
        ::-webkit-scrollbar-thumb { background: #334155; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #8B5CF6; }
    </style>
</head>
<body class="bg-brand-dark text-slate-100 min-h-screen selection:bg-brand-purple selection:text-white relative overflow-x-hidden">

    <!-- NAVIGATION BAR -->
    <header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4">
            <div class="glass-card rounded-2xl px-5 py-3 flex items-center justify-between shadow-2xl">
                <!-- Logo -->
                <a href="#" class="flex items-center gap-3 group">
                    <div class="w-10 h-10 rounded-xl bg-gradient-brand flex items-center justify-center text-white font-extrabold text-xl shadow-lg shadow-purple-500/30 group-hover:scale-105 transition-transform">
                        AR
                    </div>
                    <div>
                        <span class="font-bold text-lg tracking-tight block leading-none">Alex Rivera</span>
                        <span class="text-xs text-brand-cyan font-medium">Social Strategist</span>
                    </div>
                </a>

                <!-- Desktop Nav Links -->
                <nav class="hidden md:flex items-center space-x-8 font-medium text-sm text-slate-300">
                    <a href="#about" class="hover:text-brand-pink transition-colors">About & Skills</a>
                    <a href="#portfolio" class="hover:text-brand-purple transition-colors">Case Studies</a>
                    <a href="#tools" class="hover:text-brand-cyan transition-colors">Interactive Tools</a>
                    <a href="#pricing" class="hover:text-brand-pink transition-colors">Packages</a>
                    <a href="#testimonials" class="hover:text-brand-purple transition-colors">Reviews</a>
                </nav>

                <!-- CTA & Mobile Toggle -->
                <div class="flex items-center gap-4">
                    <a href="#contact" class="hidden sm:inline-flex items-center gap-2 px-5 py-2.5 rounded-xl font-semibold text-sm text-white bg-gradient-brand shadow-lg shadow-purple-500/25 hover:shadow-purple-500/40 hover:scale-[1.02] active:scale-[0.98] transition-all">
                        <span>Let's Connect</span>
                        <i class="fa-solid font-xs fa-arrow-right"></i>
                    </a>
                    <button id="mobile-menu-btn" class="md:hidden text-slate-300 hover:text-white p-2 text-xl" aria-label="Toggle menu">
                        <i class="fa-solid fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu Dropdown -->
        <div id="mobile-menu" class="hidden md:hidden px-4 pt-2 pb-6 max-w-7xl mx-auto">
            <div class="glass-card rounded-2xl p-5 flex flex-col space-y-4 font-medium text-slate-200">
                <a href="#about" class="mobile-nav-link hover:text-brand-pink">About & Skills</a>
                <a href="#portfolio" class="mobile-nav-link hover:text-brand-purple">Case Studies</a>
                <a href="#tools" class="mobile-nav-link hover:text-brand-cyan">Interactive Tools</a>
                <a href="#pricing" class="mobile-nav-link hover:text-brand-pink">Packages</a>
                <a href="#testimonials" class="mobile-nav-link hover:text-brand-purple">Reviews</a>
                <a href="#contact" class="mobile-nav-link pt-2 text-center rounded-xl py-3 text-white bg-gradient-brand font-semibold">Let's Connect</a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative pt-32 pb-20 md:pt-44 md:pb-32 overflow-hidden flex items-center min-h-screen">
        <!-- Background Glowing Orbs -->
        <div class="absolute top-1/4 left-10 w-96 h-96 bg-brand-pink/20 rounded-full animate-pulse-glow pointer-events-none"></div>
        <div class="absolute bottom-10 right-10 w-[30rem] h-[30rem] bg-brand-purple/20 rounded-full animate-pulse-glow pointer-events-none" style="animation-delay: 1.5s;"></div>
        <div class="absolute top-1/3 right-1/4 w-80 h-80 bg-brand-cyan/20 rounded-full animate-pulse-glow pointer-events-none" style="animation-delay: 3s;"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 w-full">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
                
                <!-- Text Content -->
                <div class="lg:col-span-7 space-y-8 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full glass-card text-brand-cyan text-xs sm:text-sm font-semibold tracking-wide border border-brand-cyan/30">
                        <span class="w-2 h-2 rounded-full bg-brand-cyan animate-ping"></span>
                        <span>Available for Strategic Partnerships & Management</span>
                    </div>

                    <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight leading-[1.1]">
                        Elevating Brands Through <span class="text-gradient">Strategic Content</span> & Viral Growth.
                    </h1>

                    <p class="text-slate-300 text-lg sm:text-xl max-w-2xl mx-auto lg:mx-0 font-normal leading-relaxed">
                        I turn passive scrollers into passionate brand advocates. Specialized in short-form video, data-driven paid social campaigns, and community building.
                    </p>

                    <!-- Quick Stats Badges -->
                    <div class="grid grid-cols-3 gap-4 pt-2 max-w-lg mx-auto lg:mx-0">
                        <div class="glass-card p-4 rounded-2xl border-l-4 border-l-brand-pink">
                            <div class="text-2xl sm:text-3xl font-extrabold text-white counter" data-target="150">0</div>
                            <div class="text-xs sm:text-sm text-slate-400 font-medium">M+ Impressions</div>
                        </div>
                        <div class="glass-card p-4 rounded-2xl border-l-4 border-l-brand-purple">
                            <div class="text-2xl sm:text-3xl font-extrabold text-white counter" data-target="320">0</div>
                            <div class="text-xs sm:text-sm text-slate-400 font-medium">% Avg ER Boost</div>
                        </div>
                        <div class="glass-card p-4 rounded-2xl border-l-4 border-l-brand-cyan">
                            <div class="text-2xl sm:text-3xl font-extrabold text-white counter" data-target="6">0</div>
                            <div class="text-xs sm:text-sm text-slate-400 font-medium">Yrs Experience</div>
                        </div>
                    </div>

                    <!-- Call To Action Buttons -->
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
                        <a href="#portfolio" class="w-full sm:w-auto px-8 py-4 rounded-xl font-bold text-white bg-gradient-brand shadow-xl shadow-purple-500/30 hover:scale-105 active:scale-95 transition-all text-center flex items-center justify-center gap-3">
                            <i class="fa-solid fa-layer-group"></i>
                            <span>Explore Case Studies</span>
                        </a>
                        <a href="#tools" class="w-full sm:w-auto px-8 py-4 rounded-xl font-semibold text-slate-200 glass-card hover:bg-slate-800 hover:text-white transition-all text-center border border-slate-700 flex items-center justify-center gap-2">
                            <i class="fa-solid fa-calculator text-brand-cyan"></i>
                            <span>Try ER Calculator</span>
                        </a>
                    </div>
                </div>

                <!-- Hero Visual / Profile Card -->
                <div class="lg:col-span-5 flex justify-center">
                    <div class="relative w-full max-w-md animate-float">
                        <!-- Animated Gradient Border Ring -->
                        <div class="absolute -inset-1.5 bg-gradient-brand rounded-3xl blur-lg opacity-75 animate-pulse"></div>
                        
                        <div class="relative glass-card rounded-3xl p-6 overflow-hidden border border-slate-700/60 shadow-2xl">
                            <!-- Avatar Placeholder -->
                            <div class="relative rounded-2xl overflow-hidden aspect-square mb-6 bg-slate-800 group">
                                <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=800&q=80" 
                                     alt="Alex Rivera - Social Media Strategist" 
                                     class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                                     onerror="this.onerror=null; this.src='https://placehold.co/600x600/1e293b/ffffff?text=Alex+Rivera';">
                                <div class="absolute inset-0 bg-gradient-to-t from-slate-950/80 via-transparent to-transparent"></div>
                                <div class="absolute bottom-4 left-4 right-4 flex justify-between items-end">
                                    <span class="px-3 py-1 bg-black/60 backdrop-blur-md rounded-full text-xs font-semibold text-brand-pink border border-brand-pink/30">
                                        🔥 @alex_social
                                    </span>
                                    <div class="flex gap-2">
                                        <span class="w-8 h-8 rounded-full bg-black/60 backdrop-blur-md flex items-center justify-center text-xs text-white">
                                            <i class="fa-brands fa-instagram"></i>
                                        </span>
                                        <span class="w-8 h-8 rounded-full bg-black/60 backdrop-blur-md flex items-center justify-center text-xs text-white">
                                            <i class="fa-brands fa-tiktok"></i>
                                        </span>
                                    </div>
                                </div>
                            </div>

                            <!-- Floating Badge 1 -->
                            <div class="absolute -top-4 -right-4 glass-card px-4 py-2.5 rounded-2xl border border-brand-purple/40 shadow-xl flex items-center gap-3">
                                <div class="w-8 h-8 rounded-full bg-purple-500/20 text-brand-purple flex items-center justify-center text-sm font-bold">🚀</div>
                                <div>
                                    <p class="text-[10px] text-slate-400 uppercase font-bold tracking-wider">Viral Campaign</p>
                                    <p class="text-xs font-bold text-white">4.8M Views in 48h</p>
                                </div>
                            </div>

                            <!-- Floating Badge 2 -->
                            <div class="absolute bottom-10 -left-6 glass-card px-4 py-2.5 rounded-2xl border border-brand-cyan/40 shadow-xl flex items-center gap-3">
                                <div class="w-8 h-8 rounded-full bg-cyan-500/20 text-brand-cyan flex items-center justify-center text-sm font-bold">📈</div>
                                <div>
                                    <p class="text-[10px] text-slate-400 uppercase font-bold tracking-wider">Client ROI</p>
                                    <p class="text-xs font-bold text-white">12.4x Ad Spend</p>
                                </div>
                            </div>

                            <div class="space-y-2">
                                <div class="flex items-center justify-between">
                                    <h3 class="font-bold text-lg text-white">Alex Rivera</h3>
                                    <span class="text-xs text-emerald-400 font-medium flex items-center gap-1">
                                        <span class="w-2 h-2 rounded-full bg-emerald-400"></span> Online Now
                                    </span>
                                </div>
                                <p class="text-xs text-slate-300">"We don't just chase trends. We engineer viral moments grounded in brand strategy."</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- LOGO TICKER SECTION -->
    <section class="py-10 border-y border-slate-800 bg-slate-950/50 backdrop-blur-sm overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 mb-4 text-center">
            <p class="text-xs font-semibold uppercase tracking-widest text-slate-500">Trusted By Fast-Growing Brands & Industry Leaders</p>
        </div>
        
        <!-- Marquee Track -->
        <div class="flex overflow-hidden relative w-full">
            <div class="flex gap-12 whitespace-nowrap animate-ticker items-center text-slate-400 font-bold text-xl">
                <span class="flex items-center gap-2"><i class="fa-brands fa-shopify text-emerald-400"></i> SHOPIFY STORE X</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-bolt text-amber-400"></i> VOLT ENERGY</span>
                <span class="flex items-center gap-2"><i class="fa-brands fa-spotify text-emerald-500"></i> SOUNDWAVE</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-shirt text-brand-pink"></i> AURA APPAREL</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-dumbbell text-brand-cyan"></i> APEX FITNESS</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-mug-hot text-amber-600"></i> BREW & CO.</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-laptop text-brand-purple"></i> NOVA TECH</span>
                <!-- Duplicate for seamless looping -->
                <span class="flex items-center gap-2"><i class="fa-brands fa-shopify text-emerald-400"></i> SHOPIFY STORE X</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-bolt text-amber-400"></i> VOLT ENERGY</span>
                <span class="flex items-center gap-2"><i class="fa-brands fa-spotify text-emerald-500"></i> SOUNDWAVE</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-shirt text-brand-pink"></i> AURA APPAREL</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-dumbbell text-brand-cyan"></i> APEX FITNESS</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-mug-hot text-amber-600"></i> BREW & CO.</span>
                <span class="flex items-center gap-2"><i class="fa-solid fa-laptop text-brand-purple"></i> NOVA TECH</span>
            </div>
        </div>
    </section>

    <!-- ABOUT & SKILLS SECTION -->
    <section id="about" class="py-24 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-bold text-brand-cyan uppercase tracking-widest mb-3">Core Expertise</h2>
                <h3 class="text-3xl sm:text-5xl font-extrabold text-white tracking-tight">Strategy Meets Creative Execution</h3>
                <p class="mt-4 text-slate-400 text-base sm:text-lg">Combining analytical precision with trend-forward storytelling to turn modern social channels into revenue engines.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Skill Card 1 -->
                <div class="glass-card rounded-2xl p-8 hover:border-brand-pink/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-pink-500/10 border border-pink-500/30 flex items-center justify-center text-brand-pink text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-bullseye"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Content Strategy & Direction</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">Architecting omni-channel social calendars aligned with business goals, product drops, and seasonal viral opportunities.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-pink"></i> Brand Tone & Voice Frameworks</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-pink"></i> Competitive Analysis & Audits</li>
                    </ul>
                </div>

                <!-- Skill Card 2 -->
                <div class="glass-card rounded-2xl p-8 hover:border-brand-purple/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-purple-500/10 border border-purple-500/30 flex items-center justify-center text-brand-purple text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-video"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Short-Form Video (Reels/TikTok)</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">End-to-end video creation: hook writing, filming, fast-paced editing, trending audio pairing, and visual captions.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-purple"></i> CapCut / Premiere Editing</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-purple"></i> First 3-Second Hook Optimization</li>
                    </ul>
                </div>

                <!-- Skill Card 3 -->
                <div class="glass-card rounded-2xl p-8 hover:border-brand-cyan/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-cyan-500/10 border border-cyan-500/30 flex items-center justify-center text-brand-cyan text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-chart-line"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Paid Ads & Campaign Funnels</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">Creating high-converting ad creative for Meta & TikTok Ads, pixel tracking, and retargeting funnel setups.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-cyan"></i> UGC Ad Direction</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-cyan"></i> A/B Creative Testing</li>
                    </ul>
                </div>

                <!-- Skill Card 4 -->
                <div class="glass-card rounded-2xl p-8 hover:border-amber-500/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-amber-500/10 border border-amber-500/30 flex items-center justify-center text-amber-400 text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-comments"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Community & Advocacy</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">Transforming comment sections into active brand communities through active engagement, DM outreach, and influencer seeding.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-400"></i> Micro-Influencer Campaigns</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-400"></i> Crisis Management Protocols</li>
                    </ul>
                </div>

                <!-- Skill Card 5 -->
                <div class="glass-card rounded-2xl p-8 hover:border-emerald-500/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-emerald-500/10 border border-emerald-500/30 flex items-center justify-center text-emerald-400 text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-pen-nib"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Copywriting & Storytelling</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">Captivating captions, long-form LinkedIn posts, and call-to-actions that drive clicks without sounding pushy.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-emerald-400"></i> SEO & Hashtag Optimization</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-emerald-400"></i> Carousel Scriptwriting</li>
                    </ul>
                </div>

                <!-- Skill Card 6 -->
                <div class="glass-card rounded-2xl p-8 hover:border-indigo-500/50 transition-all duration-300 group hover:-translate-y-2">
                    <div class="w-14 h-14 rounded-xl bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-indigo-400 text-2xl mb-6 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-chart-pie"></i>
                    </div>
                    <h4 class="text-xl font-bold text-white mb-3">Analytics & Growth Reporting</h4>
                    <p class="text-slate-400 text-sm leading-relaxed mb-4">Custom monthly reporting dashboards focusing on reach, ER, CTR, conversion metrics, and ROI rather than vanity vanity metrics.</p>
                    <ul class="space-y-2 text-xs text-slate-300 font-medium">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-indigo-400"></i> Looker Studio & Sprout Social</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-indigo-400"></i> Actionable Content Insights</li>
                    </ul>
                </div>

            </div>
        </div>
    </section>

    <!-- PORTFOLIO / CASE STUDIES SECTION -->
    <section id="portfolio" class="py-24 bg-slate-950/40 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-12">
                <div>
                    <h2 class="text-xs font-bold text-brand-pink uppercase tracking-widest mb-3">Proven Results</h2>
                    <h3 class="text-3xl sm:text-5xl font-extrabold text-white tracking-tight">Featured Case Studies</h3>
                </div>
                <p class="text-slate-400 max-w-md mt-4 md:mt-0 text-sm">Real campaigns, verified metric growth, and creative strategy breakouts across various niches.</p>
            </div>

            <!-- Filter Buttons -->
            <div class="flex flex-wrap gap-2 mb-10" id="portfolio-filters">
                <button class="filter-btn active px-5 py-2.5 rounded-xl font-semibold text-xs sm:text-sm bg-gradient-brand text-white shadow-lg transition-all" data-filter="all">All Platforms</button>
                <button class="filter-btn px-5 py-2.5 rounded-xl font-semibold text-xs sm:text-sm glass-card text-slate-300 hover:text-white hover:bg-slate-800 transition-all" data-filter="instagram"><i class="fa-brands fa-instagram mr-1"></i> Instagram</button>
                <button class="filter-btn px-5 py-2.5 rounded-xl font-semibold text-xs sm:text-sm glass-card text-slate-300 hover:text-white hover:bg-slate-800 transition-all" data-filter="tiktok"><i class="fa-brands fa-tiktok mr-1"></i> TikTok</button>
                <button class="filter-btn px-5 py-2.5 rounded-xl font-semibold text-xs sm:text-sm glass-card text-slate-300 hover:text-white hover:bg-slate-800 transition-all" data-filter="linkedin"><i class="fa-brands fa-linkedin mr-1"></i> LinkedIn</button>
                <button class="filter-btn px-5 py-2.5 rounded-xl font-semibold text-xs sm:text-sm glass-card text-slate-300 hover:text-white hover:bg-slate-800 transition-all" data-filter="paid"><i class="fa-solid fa-rectangle-ad mr-1"></i> Paid Ads</button>
            </div>

            <!-- Portfolio Cards Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8" id="portfolio-grid">
                
                <!-- Case Study 1: TikTok & Reels Viral Growth -->
                <div class="portfolio-card glass-card rounded-2xl overflow-hidden border border-slate-700/50 group flex flex-col" data-category="tiktok instagram">
                    <div class="relative h-60 overflow-hidden bg-slate-900">
                        <img src="https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80" 
                             alt="Aura Apparel Viral Launch" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/20 to-transparent"></div>
                        <span class="absolute top-4 left-4 bg-brand-pink text-white text-xs font-bold px-3 py-1 rounded-full flex items-center gap-1">
                            <i class="fa-brands fa-tiktok"></i> TikTok & Reels
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between">
                        <div>
                            <p class="text-xs text-brand-pink font-semibold uppercase tracking-wider mb-1">E-Commerce Fashion</p>
                            <h4 class="text-xl font-bold text-white mb-2">Aura Apparel Viral Launch</h4>
                            <p class="text-slate-400 text-sm line-clamp-2 mb-4">Leveraged audio trends & micro-influencer UGC to launch their summer streetwear drop.</p>
                            
                            <!-- Metrics Pill Grid -->
                            <div class="grid grid-cols-2 gap-2 mb-6">
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">Total Views</div>
                                    <div class="text-base font-extrabold text-brand-pink">+8.4M</div>
                                </div>
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">Follower Growth</div>
                                    <div class="text-base font-extrabold text-brand-cyan">+45.2K</div>
                                </div>
                            </div>
                        </div>

                        <button onclick="openModal('case1')" class="w-full py-3 rounded-xl bg-slate-800 hover:bg-gradient-brand text-white text-xs font-bold transition-all flex items-center justify-center gap-2">
                            <span>View Full Case Study</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <!-- Case Study 2: LinkedIn Thought Leadership -->
                <div class="portfolio-card glass-card rounded-2xl overflow-hidden border border-slate-700/50 group flex flex-col" data-category="linkedin">
                    <div class="relative h-60 overflow-hidden bg-slate-900">
                        <img src="https://images.unsplash.com/photo-1551836022-d5d88e9218df?auto=format&fit=crop&w=800&q=80" 
                             alt="Nova Tech Founder Branding" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/20 to-transparent"></div>
                        <span class="absolute top-4 left-4 bg-blue-600 text-white text-xs font-bold px-3 py-1 rounded-full flex items-center gap-1">
                            <i class="fa-brands fa-linkedin"></i> LinkedIn
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between">
                        <div>
                            <p class="text-xs text-blue-400 font-semibold uppercase tracking-wider mb-1">B2B SaaS</p>
                            <h4 class="text-xl font-bold text-white mb-2">Nova Tech Founder Branding</h4>
                            <p class="text-slate-400 text-sm line-clamp-2 mb-4">Positioning CEO as an AI thought leader using interactive carousel decks and storytelling.</p>
                            
                            <!-- Metrics Pill Grid -->
                            <div class="grid grid-cols-2 gap-2 mb-6">
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">Inbound Leads</div>
                                    <div class="text-base font-extrabold text-blue-400">+120/mo</div>
                                </div>
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">Impression Growth</div>
                                    <div class="text-base font-extrabold text-brand-purple">+620%</div>
                                </div>
                            </div>
                        </div>

                        <button onclick="openModal('case2')" class="w-full py-3 rounded-xl bg-slate-800 hover:bg-gradient-brand text-white text-xs font-bold transition-all flex items-center justify-center gap-2">
                            <span>View Full Case Study</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <!-- Case Study 3: Paid Ad Meta Scaling -->
                <div class="portfolio-card glass-card rounded-2xl overflow-hidden border border-slate-700/50 group flex flex-col" data-category="paid instagram">
                    <div class="relative h-60 overflow-hidden bg-slate-900">
                        <img src="https://images.unsplash.com/photo-1517838277536-f5f99be501cd?auto=format&fit=crop&w=800&q=80" 
                             alt="Apex Fitness Campaign" 
                             class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/20 to-transparent"></div>
                        <span class="absolute top-4 left-4 bg-brand-cyan text-white text-xs font-bold px-3 py-1 rounded-full flex items-center gap-1">
                            <i class="fa-solid fa-rectangle-ad"></i> Meta Paid Ads
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between">
                        <div>
                            <p class="text-xs text-brand-cyan font-semibold uppercase tracking-wider mb-1">Fitness & Health</p>
                            <h4 class="text-xl font-bold text-white mb-2">Apex Fitness App Scaled</h4>
                            <p class="text-slate-400 text-sm line-clamp-2 mb-4">High-converting UGC ads combined with retargeting strategy for annual sub offers.</p>
                            
                            <!-- Metrics Pill Grid -->
                            <div class="grid grid-cols-2 gap-2 mb-6">
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">ROAS</div>
                                    <div class="text-base font-extrabold text-emerald-400">4.8x</div>
                                </div>
                                <div class="bg-slate-800/80 p-2.5 rounded-xl border border-slate-700">
                                    <div class="text-xs text-slate-400">New App Installs</div>
                                    <div class="text-base font-extrabold text-brand-cyan">38,000+</div>
                                </div>
                            </div>
                        </div>

                        <button onclick="openModal('case3')" class="w-full py-3 rounded-xl bg-slate-800 hover:bg-gradient-brand text-white text-xs font-bold transition-all flex items-center justify-center gap-2">
                            <span>View Full Case Study</span>
                            <i class="fa-solid fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- INTERACTIVE TOOLS SECTION -->
    <section id="tools" class="py-24 relative overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-bold text-brand-purple uppercase tracking-widest mb-3">Bonus Interactive Tools</h2>
                <h3 class="text-3xl sm:text-5xl font-extrabold text-white tracking-tight">Social Growth & ROI Calculators</h3>
                <p class="mt-4 text-slate-400 text-base">Test your brand's current engagement health or estimate potential ROI from managed campaigns.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                
                <!-- TOOL 1: Engagement Rate Calculator -->
                <div class="glass-card rounded-3xl p-8 border border-slate-700/80 relative">
                    <div class="flex items-center gap-3 mb-6">
                        <div class="w-12 h-12 rounded-xl bg-purple-500/20 text-brand-purple flex items-center justify-center text-xl">
                            <i class="fa-solid fa-calculator"></i>
                        </div>
                        <div>
                            <h4 class="text-xl font-bold text-white">Engagement Rate Calculator</h4>
                            <p class="text-xs text-slate-400">Calculate average engagement per post</p>
                        </div>
                    </div>

                    <div class="space-y-4">
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">Total Followers</label>
                            <input type="number" id="er-followers" value="25000" placeholder="e.g. 25000" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white focus:outline-none focus:border-brand-purple text-sm">
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-xs font-medium text-slate-300 mb-1">Avg Likes / Post</label>
                                <input type="number" id="er-likes" value="1200" placeholder="e.g. 1200" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white focus:outline-none focus:border-brand-purple text-sm">
                            </div>
                            <div>
                                <label class="block text-xs font-medium text-slate-300 mb-1">Avg Comments / Post</label>
                                <input type="number" id="er-comments" value="150" placeholder="e.g. 150" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white focus:outline-none focus:border-brand-purple text-sm">
                            </div>
                        </div>

                        <button id="calc-er-btn" class="w-full py-3 rounded-xl bg-gradient-brand text-white font-bold text-sm shadow-lg hover:opacity-90 transition-all mt-2">
                            Calculate ER Benchmark
                        </button>

                        <!-- ER Result Box -->
                        <div id="er-result" class="mt-4 p-4 rounded-2xl bg-slate-900/80 border border-slate-800 flex items-center justify-between">
                            <div>
                                <div class="text-xs text-slate-400">Estimated Engagement Rate</div>
                                <div class="text-2xl font-black text-brand-purple" id="er-score">5.40%</div>
                            </div>
                            <div class="text-right">
                                <span class="px-3 py-1 rounded-full text-xs font-bold bg-emerald-500/20 text-emerald-400 border border-emerald-500/30" id="er-badge">Excellent 🔥</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- TOOL 2: Campaign Reach & Leads Estimator -->
                <div class="glass-card rounded-3xl p-8 border border-slate-700/80 relative">
                    <div class="flex items-center gap-3 mb-6">
                        <div class="w-12 h-12 rounded-xl bg-pink-500/20 text-brand-pink flex items-center justify-center text-xl">
                            <i class="fa-solid fa-sliders"></i>
                        </div>
                        <div>
                            <h4 class="text-xl font-bold text-white">Organic & Paid Growth Estimator</h4>
                            <p class="text-xs text-slate-400">Estimate monthly reach & lead potential based on budget</p>
                        </div>
                    </div>

                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between text-xs font-medium text-slate-300 mb-2">
                                <span>Monthly Ad/Content Budget ($)</span>
                                <span class="text-brand-pink font-bold" id="budget-value">$2,500</span>
                            </div>
                            <input type="range" id="budget-range" min="500" max="10000" step="500" value="2500" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer accent-brand-pink">
                        </div>

                        <div>
                            <div class="flex justify-between text-xs font-medium text-slate-300 mb-2">
                                <span>Target Channel Goal</span>
                                <span class="text-brand-cyan font-bold" id="channel-target">Viral Short-Form Video</span>
                            </div>
                            <select id="channel-select" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white focus:outline-none focus:border-brand-pink text-sm">
                                <option value="shortform">Short-Form Video (TikTok/Reels)</option>
                                <option value="paid">Meta & TikTok Paid Acquisition</option>
                                <option value="b2b">LinkedIn B2B Organic Lead Gen</option>
                            </select>
                        </div>

                        <!-- ROI Results Card -->
                        <div class="grid grid-cols-2 gap-4 pt-2">
                            <div class="bg-slate-900/80 p-4 rounded-2xl border border-slate-800">
                                <div class="text-xs text-slate-400">Estimated Monthly Impressions</div>
                                <div class="text-xl font-extrabold text-brand-pink" id="est-reach">250K - 500K</div>
                            </div>
                            <div class="bg-slate-900/80 p-4 rounded-2xl border border-slate-800">
                                <div class="text-xs text-slate-400">Est. Leads / Conversions</div>
                                <div class="text-xl font-extrabold text-brand-cyan" id="est-leads">120 - 280</div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- PRICING & SERVICES SECTION -->
    <section id="pricing" class="py-24 bg-slate-950/60 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-bold text-brand-cyan uppercase tracking-widest mb-3">Transparent Investment</h2>
                <h3 class="text-3xl sm:text-5xl font-extrabold text-white tracking-tight">Social Management Packages</h3>
                <p class="mt-4 text-slate-400 text-base">Tailored strategy packages designed to match your brand's growth stage.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Package 1 -->
                <div class="glass-card rounded-3xl p-8 border border-slate-800 flex flex-col justify-between hover:border-slate-600 transition-all">
                    <div>
                        <div class="text-xs font-bold uppercase tracking-wider text-slate-400 mb-2">Starter Growth</div>
                        <h4 class="text-2xl font-bold text-white mb-4">Organic Core</h4>
                        <div class="text-4xl font-extrabold text-white mb-6">$1,800<span class="text-sm font-normal text-slate-400">/mo</span></div>
                        <p class="text-slate-400 text-xs mb-6">Perfect for emerging brands needing consistent, high-quality social presence.</p>

                        <ul class="space-y-3 text-xs text-slate-300 mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-cyan"></i> 12 Original Short-Form Videos / mo</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-cyan"></i> Custom Captions & Hashtag Optimization</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-cyan"></i> Instagram & TikTok Posting Management</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-cyan"></i> Community Engagement (3 hrs/wk)</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-cyan"></i> Monthly Performance Report</li>
                        </ul>
                    </div>

                    <a href="#contact" class="w-full py-3.5 rounded-xl border border-slate-700 text-white font-bold text-xs text-center hover:bg-slate-800 transition-all">Select Organic Core</a>
                </div>

                <!-- Package 2: Featured -->
                <div class="glass-card rounded-3xl p-8 border-2 border-brand-purple relative flex flex-col justify-between shadow-2xl shadow-purple-900/20 scale-105 z-10 bg-slate-900/90">
                    <span class="absolute -top-3.5 left-1/2 -translate-x-1/2 bg-gradient-brand text-white text-[10px] uppercase font-extrabold tracking-wider px-4 py-1 rounded-full shadow-lg">Most Popular</span>
                    
                    <div>
                        <div class="text-xs font-bold uppercase tracking-wider text-brand-purple mb-2">Full-Scale Scaling</div>
                        <h4 class="text-2xl font-bold text-white mb-4">Omni-Growth Engine</h4>
                        <div class="text-4xl font-extrabold text-white mb-6">$3,500<span class="text-sm font-normal text-slate-400">/mo</span></div>
                        <p class="text-slate-400 text-xs mb-6">Designed for brands ready to dominate short-form video and scale community conversion.</p>

                        <ul class="space-y-3 text-xs text-slate-300 mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-purple"></i> 24 Short-Form Videos (Reels/TikTok/Shorts)</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-purple"></i> Influencer / UGC Gifting Strategy</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-purple"></i> Dedicated Community Manager (7 hrs/wk)</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-purple"></i> Meta & TikTok Paid Ad Creative Direction</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-purple"></i> Bi-Weekly Strategy Call & Live Reporting</li>
                        </ul>
                    </div>

                    <a href="#contact" class="w-full py-3.5 rounded-xl bg-gradient-brand text-white font-bold text-xs text-center shadow-lg hover:scale-105 transition-all">Claim Growth Engine</a>
                </div>

                <!-- Package 3 -->
                <div class="glass-card rounded-3xl p-8 border border-slate-800 flex flex-col justify-between hover:border-slate-600 transition-all">
                    <div>
                        <div class="text-xs font-bold uppercase tracking-wider text-slate-400 mb-2">VIP Custom Launch</div>
                        <h4 class="text-2xl font-bold text-white mb-4">Campaign Takeover</h4>
                        <div class="text-4xl font-extrabold text-white mb-6">$5,500+<span class="text-sm font-normal text-slate-400">/project</span></div>
                        <p class="text-slate-400 text-xs mb-6">Intensive product launch, rebrand, or event-based viral social push.</p>

                        <ul class="space-y-3 text-xs text-slate-300 mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-pink"></i> Full Product Launch Strategy & Scripting</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-pink"></i> On-site Video Production Crew Coordination</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-pink"></i> Paid Ad Funnel Setup & Meta Scaling</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-pink"></i> Tier-1 Influencer Seeding</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-brand-pink"></i> 24/7 Crisis & Campaign Analytics Room</li>
                        </ul>
                    </div>

                    <a href="#contact" class="w-full py-3.5 rounded-xl border border-slate-700 text-white font-bold text-xs text-center hover:bg-slate-800 transition-all">Request VIP Proposal</a>
                </div>

            </div>
        </div>
    </section>

    <!-- TESTIMONIALS SECTION -->
    <section id="testimonials" class="py-24 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-bold text-brand-pink uppercase tracking-widest mb-3">Client Feedback</h2>
                <h3 class="text-3xl sm:text-5xl font-extrabold text-white tracking-tight">What Founders & CMOs Say</h3>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <div class="glass-card rounded-2xl p-8 relative flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="flex text-amber-400 gap-1 text-sm">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">"Alex completely transformed our TikTok presence from non-existent to generating 30% of our organic e-commerce revenue within 90 days."</p>
                    </div>
                    <div class="flex items-center gap-3 pt-6 border-t border-slate-800 mt-6">
                        <img src="https://images.unsplash.com/photo-1580489944761-15a19d654956?auto=format&fit=crop&w=150&q=80" alt="Sarah Jenkins" class="w-10 h-10 rounded-full object-cover">
                        <div>
                            <h5 class="text-sm font-bold text-white">Sarah Jenkins</h5>
                            <p class="text-xs text-slate-400">CMO @ Aura Apparel</p>
                        </div>
                    </div>
                </div>

                <div class="glass-card rounded-2xl p-8 relative flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="flex text-amber-400 gap-1 text-sm">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">"The LinkedIn thought leadership strategy doubled our enterprise demo requests. Alex knows how to write for C-suite audiences without sounding robotic."</p>
                    </div>
                    <div class="flex items-center gap-3 pt-6 border-t border-slate-800 mt-6">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=150&q=80" alt="Marcus Vance" class="w-10 h-10 rounded-full object-cover">
                        <div>
                            <h5 class="text-sm font-bold text-white">Marcus Vance</h5>
                            <p class="text-xs text-slate-400">Founder @ Nova Tech</p>
                        </div>
                    </div>
                </div>

                <div class="glass-card rounded-2xl p-8 relative flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="flex text-amber-400 gap-1 text-sm">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                        </div>
                        <p class="text-slate-300 text-sm leading-relaxed italic">"Working with Alex felt like having an entire in-house social agency for a fraction of the cost. Creative, communicative, and insanely performance-driven."</p>
                    </div>
                    <div class="flex items-center gap-3 pt-6 border-t border-slate-800 mt-6">
                        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=150&q=80" alt="Elena Rostova" class="w-10 h-10 rounded-full object-cover">
                        <div>
                            <h5 class="text-sm font-bold text-white">Elena Rostova</h5>
                            <p class="text-xs text-slate-400">Marketing Director @ Apex Fitness</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section id="contact" class="py-24 bg-slate-950 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Contact Info -->
                <div class="lg:col-span-5 space-y-6">
                    <h2 class="text-xs font-bold text-brand-cyan uppercase tracking-widest">Let's Connect</h2>
                    <h3 class="text-4xl font-extrabold text-white tracking-tight">Ready to scale your social footprint?</h3>
                    <p class="text-slate-300 text-sm leading-relaxed">Fill out the brief form or schedule a free 20-minute social audit call to discuss your growth goals.</p>

                    <div class="space-y-4 pt-4">
                        <div class="flex items-center gap-4 text-slate-300 text-sm">
                            <div class="w-10 h-10 rounded-xl bg-slate-900 border border-slate-800 flex items-center justify-center text-brand-pink">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <span>alex.rivera@socialstrategy.io</span>
                        </div>
                        <div class="flex items-center gap-4 text-slate-300 text-sm">
                            <div class="w-10 h-10 rounded-xl bg-slate-900 border border-slate-800 flex items-center justify-center text-brand-purple">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <span>Los Angeles, CA (Available Worldwide)</span>
                        </div>
                    </div>

                    <!-- Social Media Links -->
                    <div class="pt-6">
                        <p class="text-xs font-semibold text-slate-400 uppercase tracking-wider mb-4">Follow My Personal Socials</p>
                        <div class="flex gap-3">
                            <a href="#" class="w-10 h-10 rounded-xl glass-card flex items-center justify-center text-slate-300 hover:text-white hover:bg-brand-pink transition-all">
                                <i class="fa-brands fa-instagram"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-xl glass-card flex items-center justify-center text-slate-300 hover:text-white hover:bg-black transition-all">
                                <i class="fa-brands fa-tiktok"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-xl glass-card flex items-center justify-center text-slate-300 hover:text-white hover:bg-blue-600 transition-all">
                                <i class="fa-brands fa-linkedin-in"></i>
                            </a>
                            <a href="#" class="w-10 h-10 rounded-xl glass-card flex items-center justify-center text-slate-300 hover:text-white hover:bg-cyan-500 transition-all">
                                <i class="fa-brands fa-x-twitter"></i>
                            </a>
                        </div>
                    </div>
                </div>

                <!-- Interactive Contact Form -->
                <div class="lg:col-span-7">
                    <div class="glass-card rounded-3xl p-8 border border-slate-800 shadow-2xl relative">
                        <form id="contact-form" class="space-y-4">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-medium text-slate-300 mb-1">Your Name *</label>
                                    <input type="text" required placeholder="Jane Doe" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-purple">
                                </div>
                                <div>
                                    <label class="block text-xs font-medium text-slate-300 mb-1">Email Address *</label>
                                    <input type="email" required placeholder="jane@brand.com" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-purple">
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-medium text-slate-300 mb-1">Brand Name / Website</label>
                                    <input type="text" placeholder="www.yourbrand.com" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-purple">
                                </div>
                                <div>
                                    <label class="block text-xs font-medium text-slate-300 mb-1">Estimated Budget</label>
                                    <select class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-purple">
                                        <option>$1,500 - $3,000 / mo</option>
                                        <option>$3,000 - $5,000 / mo</option>
                                        <option>$5,000+ / mo</option>
                                        <option>One-Time Project Launch</option>
                                    </select>
                                </div>
                            </div>

                            <div>
                                <label class="block text-xs font-medium text-slate-300 mb-1">What are your main social media goals?</label>
                                <textarea rows="4" required placeholder="Tell me about your brand, current bottlenecks, and targets..." class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-purple"></textarea>
                            </div>

                            <button type="submit" class="w-full py-4 rounded-xl bg-gradient-brand text-white font-bold text-sm shadow-xl shadow-purple-500/20 hover:scale-[1.01] transition-all flex items-center justify-center gap-2">
                                <i class="fa-solid fa-paper-plane"></i>
                                <span>Send Inquiry & Schedule Call</span>
                            </button>
                        </form>

                        <!-- Success Message Banner -->
                        <div id="form-success" class="hidden absolute inset-0 glass-card bg-slate-950/95 rounded-3xl p-8 flex flex-col items-center justify-center text-center space-y-4">
                            <div class="w-16 h-16 rounded-full bg-emerald-500/20 text-emerald-400 flex items-center justify-center text-3xl">
                                <i class="fa-solid fa-check"></i>
                            </div>
                            <h4 class="text-2xl font-bold text-white">Message Received!</h4>
                            <p class="text-slate-300 text-sm max-w-sm">Thanks for reaching out! I'll review your brand's profile and reply within 24 hours.</p>
                            <button onclick="resetForm()" class="px-6 py-2.5 rounded-xl bg-slate-800 text-xs font-bold text-white hover:bg-slate-700 transition-all">Send Another Message</button>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="py-8 border-t border-slate-800/80 text-center text-slate-500 text-xs">
        <div class="max-w-7xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-4">
            <p>© 2026 Alex Rivera. All rights reserved. Designed for Modern Social Strategy.</p>
            <div class="flex gap-6">
                <a href="#" class="hover:text-slate-300">Privacy Policy</a>
                <a href="#" class="hover:text-slate-300">Terms of Service</a>
            </div>
        </div>
    </footer>

    <!-- CASE STUDY MODAL -->
    <div id="case-modal" class="fixed inset-0 z-50 hidden bg-black/80 backdrop-blur-md flex items-center justify-center p-4 overflow-y-auto">
        <div class="glass-card rounded-3xl max-w-3xl w-full p-6 sm:p-8 border border-slate-700 relative max-h-[90vh] overflow-y-auto">
            <button onclick="closeModal()" class="absolute top-6 right-6 text-slate-400 hover:text-white text-xl">
                <i class="fa-solid fa-xmark"></i>
            </button>

            <div id="modal-content">
                <!-- Modal content dynamically injected via JavaScript -->
            </div>
        </div>
    </div>

    <!-- JAVASCRIPT INTERACTION LOGIC -->
    <script>
        // 1. Mobile Menu Toggle
        const menuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileNavLinks = document.querySelectorAll('.mobile-nav-link');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        mobileNavLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // 2. Animated Counter Effect
        const counters = document.querySelectorAll('.counter');
        let counterTriggered = false;

        function runCounters() {
            counters.forEach(counter => {
                const target = +counter.getAttribute('data-target');
                let count = 0;
                const speed = target / 50;

                const updateCount = () => {
                    count += speed;
                    if (count < target) {
                        counter.innerText = Math.ceil(count);
                        setTimeout(updateCount, 25);
                    } else {
                        counter.innerText = target;
                    }
                };
                updateCount();
            });
        }

        // Trigger counter on scroll
        window.addEventListener('scroll', () => {
            const heroPos = document.getElementById('about').getBoundingClientRect().top;
            if (heroPos < window.innerHeight && !counterTriggered) {
                runCounters();
                counterTriggered = true;
            }
        });
        // Initial run in case on screen
        runCounters();

        // 3. Portfolio Filter Tabs
        const filterBtns = document.querySelectorAll('.filter-btn');
        const portfolioCards = document.querySelectorAll('.portfolio-card');

        filterBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                filterBtns.forEach(b => {
                    b.classList.remove('active', 'bg-gradient-brand', 'text-white');
                    b.classList.add('glass-card', 'text-slate-300');
                });
                btn.classList.add('active', 'bg-gradient-brand', 'text-white');
                btn.classList.remove('glass-card', 'text-slate-300');

                const filter = btn.getAttribute('data-filter');

                portfolioCards.forEach(card => {
                    if (filter === 'all' || card.getAttribute('data-category').includes(filter)) {
                        card.style.display = 'flex';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });

        // 4. Case Study Modal Data & Functions
        const modalData = {
            case1: {
                title: "Aura Apparel: 0 to 8.4M Views Short-Form Strategy",
                category: "TikTok & Instagram Reels Campaign",
                summary: "Aura Apparel needed an organic social revival ahead of their summer clothing line drop without relying heavily on paid ad budget.",
                strategy: [
                    "Identified 15 emerging audio trends tailored to Gen-Z streetwear fashion.",
                    "Coordinated UGC product gifting with 25 micro-creators.",
                    "Optimized dynamic first-3-second video hooks focusing on outfit transformations."
                ],
                results: [
                    "8.4M Total Organic Impressions in 30 Days",
                    "+45,200 Instagram & TikTok Followers Gained",
                    "$68,000 Direct Sales tracked via bio link discount codes"
                ]
            },
            case2: {
                title: "Nova Tech: B2B LinkedIn Thought Leadership",
                category: "Executive Personal Branding",
                summary: "Positioned Nova Tech's founder as a leading voice in AI automation, targeting SaaS buyers and enterprise leads.",
                strategy: [
                    "Authored 4 high-value text/carousel posts per week synthesizing AI industry trends.",
                    "Engaged daily with key decision-makers' comment threads.",
                    "Designed high-contrast, clean visual carousels with strong CTAs."
                ],
                results: [
                    "+620% Increase in Profile Impressions",
                    "120+ Inbound Demo Requests directly from LinkedIn outreach",
                    "Featured in major industry newsletters as Top Tech Founder to watch"
                ]
            },
            case3: {
                title: "Apex Fitness: Meta Paid Social Scaling Strategy",
                category: "Paid Ads & UGC Acquisition",
                summary: "Scaled subscriber acquisition for a high-intensity workout mobile app via high-converting Meta and TikTok video ad creative.",
                strategy: [
                    "A/B tested 12 unique hook variations focusing on workout transformations and pain points.",
                    "Implemented retargeting creative sequence for users abandoning checkout.",
                    "Built custom campaign audiences based on high-LTV workout enthusiasts."
                ],
                results: [
                    "4.8x Return on Ad Spend (ROAS)",
                    "38,000+ New Fitness App Installs",
                    "Reduced Cost Per Acquisition (CPA) by 34%"
                ]
            }
        };

        function openModal(caseKey) {
            const data = modalData[caseKey];
            const modalContent = document.getElementById('modal-content');

            modalContent.innerHTML = `
                <span class="text-xs font-bold text-brand-pink uppercase tracking-widest">${data.category}</span>
                <h3 class="text-2xl sm:text-3xl font-extrabold text-white mt-1 mb-4">${data.title}</h3>
                
                <p class="text-slate-300 text-sm leading-relaxed mb-6">${data.summary}</p>
                
                <div class="space-y-6">
                    <div>
                        <h4 class="text-sm font-bold text-brand-cyan uppercase tracking-wider mb-2">Core Execution Strategy</h4>
                        <ul class="space-y-2 text-xs text-slate-300">
                            ${data.strategy.map(item => `<li class="flex items-start gap-2"><i class="fa-solid fa-angle-right text-brand-purple mt-0.5"></i> ${item}</li>`).join('')}
                        </ul>
                    </div>

                    <div>
                        <h4 class="text-sm font-bold text-emerald-400 uppercase tracking-wider mb-2">Verified Key Metrics</h4>
                        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                            ${data.results.map(res => `<div class="bg-slate-900 p-3 rounded-xl border border-slate-800 text-xs font-bold text-white">${res}</div>`).join('')}
                        </div>
                    </div>
                </div>

                <div class="mt-8 pt-6 border-t border-slate-800 flex justify-end">
                    <button onclick="closeModal()" class="px-6 py-2.5 rounded-xl bg-gradient-brand text-white font-bold text-xs">Close Preview</button>
                </div>
            `;

            document.getElementById('case-modal').classList.remove('hidden');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            document.getElementById('case-modal').classList.add('hidden');
            document.body.style.overflow = 'auto';
        }

        // 5. Engagement Rate Calculator Logic
        const calcErBtn = document.getElementById('calc-er-btn');
        calcErBtn.addEventListener('click', () => {
            const followers = parseFloat(document.getElementById('er-followers').value) || 1;
            const likes = parseFloat(document.getElementById('er-likes').value) || 0;
            const comments = parseFloat(document.getElementById('er-comments').value) || 0;

            const er = (((likes + comments) / followers) * 100).toFixed(2);
            document.getElementById('er-score').innerText = er + '%';

            const badge = document.getElementById('er-badge');
            if (er >= 3.5) {
                badge.innerText = 'Excellent 🔥';
                badge.className = 'px-3 py-1 rounded-full text-xs font-bold bg-emerald-500/20 text-emerald-400 border border-emerald-500/30';
            } else if (er >= 1.5) {
                badge.innerText = 'Average 👍';
                badge.className = 'px-3 py-1 rounded-full text-xs font-bold bg-amber-500/20 text-amber-400 border border-amber-500/30';
            } else {
                badge.innerText = 'Needs Boost 🚀';
                badge.className = 'px-3 py-1 rounded-full text-xs font-bold bg-rose-500/20 text-rose-400 border border-rose-500/30';
            }
        });

        // 6. Campaign Growth Estimator Slider Logic
        const budgetRange = document.getElementById('budget-range');
        const budgetValue = document.getElementById('budgetValue');
        const channelSelect = document.getElementById('channel-select');
        const estReach = document.getElementById('est-reach');
        const estLeads = document.getElementById('est-leads');

        function updateEstimator() {
            const val = parseInt(budgetRange.value);
            document.getElementById('budget-value').innerText = '$' + val.toLocaleString();

            const channel = channelSelect.value;
            let reachMultiplier = 100;
            let leadMultiplier = 0.08;

            if (channel === 'shortform') {
                reachMultiplier = 180;
                leadMultiplier = 0.05;
            } else if (channel === 'paid') {
                reachMultiplier = 80;
                leadMultiplier = 0.12;
            } else if (channel === 'b2b') {
                reachMultiplier = 40;
                leadMultiplier = 0.09;
            }

            const minReach = Math.round((val * reachMultiplier) / 1000) * 1000;
            const maxReach = Math.round(minReach * 1.8);

            const minLeads = Math.round(val * leadMultiplier);
            const maxLeads = Math.round(minLeads * 1.6);

            estReach.innerText = `${(minReach / 1000).toFixed(0)}K - ${(maxReach / 1000).toFixed(0)}K`;
            estLeads.innerText = `${minLeads} - ${maxLeads}`;
        }

        budgetRange.addEventListener('input', updateEstimator);
        channelSelect.addEventListener('change', updateEstimator);

        // 7. Contact Form Simulation
        const contactForm = document.getElementById('contact-form');
        const formSuccess = document.getElementById('form-success');

        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            formSuccess.classList.remove('hidden');
        });

        function resetForm() {
            contactForm.reset();
            formSuccess.classList.add('hidden');
        }
    </script>
</body>
</html>
