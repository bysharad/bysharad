<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sharad | Software Engineer & Architect</title>
    
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['Fira Code', 'monospace'],
                    },
                    colors: {
                        // Tokyo Night inspired palette
                        background: '#1a1b26',
                        surface: '#24283b',
                        surfaceHighlight: '#292e42',
                        primary: '#7aa2f7',
                        secondary: '#bb9af7',
                        accent: '#0db9d7',
                        text: '#c0caf5',
                        textMuted: '#9aa5ce',
                        success: '#9ece6a',
                        warning: '#e0af68',
                        error: '#f7768e',
                    },
                    animation: {
                        'gradient-x': 'gradient-x 15s ease infinite',
                        'float': 'float 6s ease-in-out infinite',
                        'fade-in-up': 'fadeInUp 0.8s ease-out forwards',
                    },
                    keyframes: {
                        'gradient-x': {
                            '0%, 100%': {
                                'background-size': '200% 200%',
                                'background-position': 'left center'
                            },
                            '50%': {
                                'background-size': '200% 200%',
                                'background-position': 'right center'
                            },
                        },
                        'float': {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-10px)' },
                        },
                        'fadeInUp': {
                            '0%': { opacity: '0', transform: 'translateY(20px)' },
                            '100%': { opacity: '1', transform: 'translateY(0)' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #1a1b26; 
        }
        ::-webkit-scrollbar-thumb {
            background: #414868; 
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #565f89; 
        }

        body {
            background-color: #1a1b26;
            color: #c0caf5;
        }

        /* Typing cursor effect */
        .typing-cursor::after {
            content: '|';
            animation: blink 1s step-end infinite;
            color: #7aa2f7;
        }
        @keyframes blink {
            50% { opacity: 0; }
        }

        .glass-panel {
            background: rgba(36, 40, 59, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(122, 162, 247, 0.1);
        }
    </style>
</head>
<body class="antialiased min-h-screen flex flex-col items-center justify-start pt-16 pb-24 px-4 sm:px-6 lg:px-8 selection:bg-primary selection:text-background relative overflow-x-hidden">
    
    <!-- Background decorative elements -->
    <div class="fixed top-[-10%] left-[-10%] w-[40%] h-[40%] rounded-full bg-primary/10 blur-[120px] pointer-events-none"></div>
    <div class="fixed bottom-[-10%] right-[-10%] w-[40%] h-[40%] rounded-full bg-secondary/10 blur-[120px] pointer-events-none"></div>

    <main class="w-full max-w-4xl mx-auto flex flex-col items-center z-10">
        
        <!-- Header / Hero Section -->
        <div class="text-center w-full mb-12 animate-fade-in-up">
            <div class="h-24 sm:h-32 flex items-center justify-center mb-6">
                <!-- Javascript will populate this -->
                <h1 id="typewriter-text" class="font-mono text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-semibold text-primary typing-cursor min-h-[3rem]"></h1>
            </div>
            
            <p class="text-lg sm:text-xl text-textMuted font-medium mb-8 max-w-2xl mx-auto leading-relaxed">
                <span class="text-text">Architecting digital experiences</span> with zero friction and maximum impact.
            </p>

            <!-- Social Links -->
            <div class="flex flex-wrap justify-center gap-4 mb-8">
                <a href="#" class="group flex items-center gap-2 px-5 py-2.5 rounded-full bg-surface hover:bg-surfaceHighlight border border-surfaceHighlight hover:border-primary/50 transition-all duration-300 transform hover:-translate-y-1 hover:shadow-[0_0_15px_rgba(122,162,247,0.3)]">
                    <i class="fa-brands fa-linkedin text-[#0A66C2] text-xl"></i>
                    <span class="font-medium text-sm">LinkedIn</span>
                </a>
                <a href="#" class="group flex items-center gap-2 px-5 py-2.5 rounded-full bg-surface hover:bg-surfaceHighlight border border-surfaceHighlight hover:border-primary/50 transition-all duration-300 transform hover:-translate-y-1 hover:shadow-[0_0_15px_rgba(29,155,240,0.3)]">
                    <i class="fa-brands fa-twitter text-[#1D9BF0] text-xl"></i>
                    <span class="font-medium text-sm">Twitter</span>
                </a>
                <a href="#" class="group flex items-center gap-2 px-5 py-2.5 rounded-full bg-surface hover:bg-surfaceHighlight border border-surfaceHighlight hover:border-primary/50 transition-all duration-300 transform hover:-translate-y-1 hover:shadow-[0_0_15px_rgba(234,67,53,0.3)]">
                    <i class="fa-regular fa-envelope text-[#EA4335] text-xl"></i>
                    <span class="font-medium text-sm">Email</span>
                </a>
                <a href="#" class="group flex items-center gap-2 px-5 py-2.5 rounded-full bg-surface hover:bg-surfaceHighlight border border-surfaceHighlight hover:border-primary/50 transition-all duration-300 transform hover:-translate-y-1 hover:shadow-[0_0_15px_rgba(192,202,245,0.3)]">
                    <i class="fa-solid fa-globe text-text text-xl"></i>
                    <span class="font-medium text-sm">Portfolio</span>
                </a>
            </div>
        </div>

        <div class="w-full h-px bg-gradient-to-r from-transparent via-surfaceHighlight to-transparent mb-16"></div>

        <!-- Technical Arsenal Section -->
        <section class="w-full mb-16 animate-fade-in-up" style="animation-delay: 0.2s;">
            <div class="flex items-center justify-center gap-3 mb-8">
                <i class="fa-solid fa-bolt text-warning text-2xl"></i>
                <h2 class="text-2xl font-bold text-text">Technical Arsenal</h2>
            </div>
            
            <div class="glass-panel rounded-2xl p-6 sm:p-8 w-full">
                <div class="flex flex-wrap justify-center gap-3">
                    <!-- Tech Badges -->
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#3178C6]/10 border border-[#3178C6]/30 text-[#3178C6] hover:bg-[#3178C6]/20 transition-colors">
                        <i class="fa-brands fa-js-square"></i> TypeScript
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#3776AB]/10 border border-[#3776AB]/30 text-[#3776AB] hover:bg-[#3776AB]/20 transition-colors">
                        <i class="fa-brands fa-python"></i> Python
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#61DAFB]/10 border border-[#61DAFB]/30 text-[#61DAFB] hover:bg-[#61DAFB]/20 transition-colors">
                        <i class="fa-brands fa-react"></i> React
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-white/10 border border-white/30 text-white hover:bg-white/20 transition-colors">
                        <i class="fa-brands fa-node-js text-white"></i> Next.js
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#339933]/10 border border-[#339933]/30 text-[#339933] hover:bg-[#339933]/20 transition-colors">
                        <i class="fa-brands fa-node"></i> Node.js
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#4169E1]/10 border border-[#4169E1]/30 text-[#4169E1] hover:bg-[#4169E1]/20 transition-colors">
                        <i class="fa-solid fa-database"></i> PostgreSQL
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#47A248]/10 border border-[#47A248]/30 text-[#47A248] hover:bg-[#47A248]/20 transition-colors">
                        <i class="fa-solid fa-leaf"></i> MongoDB
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#2496ED]/10 border border-[#2496ED]/30 text-[#2496ED] hover:bg-[#2496ED]/20 transition-colors">
                        <i class="fa-brands fa-docker"></i> Docker
                    </span>
                    <span class="flex items-center gap-2 px-4 py-2 rounded-lg bg-[#FF9900]/10 border border-[#FF9900]/30 text-[#FF9900] hover:bg-[#FF9900]/20 transition-colors">
                        <i class="fa-brands fa-aws"></i> AWS
                    </span>
                </div>
            </div>
        </section>

        <!-- GitHub Stats Section (Stylized HTML Mockups of the typical README SVGs) -->
        <section class="w-full mb-16 animate-fade-in-up" style="animation-delay: 0.4s;">
            <div class="flex items-center justify-center gap-3 mb-8">
                <i class="fa-solid fa-chart-column text-secondary text-2xl"></i>
                <h2 class="text-2xl font-bold text-text">GitHub Analytics</h2>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 w-full mb-6">
                <!-- Stats Card -->
                <div class="glass-panel rounded-xl p-6 relative overflow-hidden group">
                    <h3 class="text-lg font-semibold text-primary mb-4 flex items-center gap-2">
                        <i class="fa-regular fa-user"></i> Sharad's GitHub Stats
                    </h3>
                    <div class="space-y-3">
                        <div class="flex justify-between items-center">
                            <span class="text-textMuted flex items-center gap-2"><i class="fa-solid fa-star text-warning w-5 text-center"></i> Total Stars Earned</span>
                            <span class="font-mono font-bold text-text">1.2k</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-textMuted flex items-center gap-2"><i class="fa-solid fa-code-commit text-primary w-5 text-center"></i> Total Commits (2024)</span>
                            <span class="font-mono font-bold text-text">842</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-textMuted flex items-center gap-2"><i class="fa-solid fa-code-pull-request text-success w-5 text-center"></i> PRs Opened</span>
                            <span class="font-mono font-bold text-text">156</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-textMuted flex items-center gap-2"><i class="fa-solid fa-box-open text-secondary w-5 text-center"></i> Issues Contributed</span>
                            <span class="font-mono font-bold text-text">43</span>
                        </div>
                    </div>
                </div>

                <!-- Top Languages Card -->
                <div class="glass-panel rounded-xl p-6 relative overflow-hidden group">
                    <h3 class="text-lg font-semibold text-primary mb-4 flex items-center gap-2">
                        <i class="fa-solid fa-laptop-code"></i> Top Languages
                    </h3>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between text-sm mb-1">
                                <span class="text-textMuted">TypeScript</span>
                                <span class="font-mono text-text">45%</span>
                            </div>
                            <div class="w-full bg-surfaceHighlight rounded-full h-2">
                                <div class="bg-[#3178C6] h-2 rounded-full" style="width: 45%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm mb-1">
                                <span class="text-textMuted">Python</span>
                                <span class="font-mono text-text">30%</span>
                            </div>
                            <div class="w-full bg-surfaceHighlight rounded-full h-2">
                                <div class="bg-[#3776AB] h-2 rounded-full" style="width: 30%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm mb-1">
                                <span class="text-textMuted">JavaScript</span>
                                <span class="font-mono text-text">15%</span>
                            </div>
                            <div class="w-full bg-surfaceHighlight rounded-full h-2">
                                <div class="bg-[#F7DF1E] h-2 rounded-full" style="width: 15%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-sm mb-1">
                                <span class="text-textMuted">HTML/CSS</span>
                                <span class="font-mono text-text">10%</span>
                            </div>
                            <div class="w-full bg-surfaceHighlight rounded-full h-2">
                                <div class="bg-[#E34F26] h-2 rounded-full" style="width: 10%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Streak Card Mockup -->
            <div class="glass-panel rounded-xl p-6 w-full max-w-2xl mx-auto flex flex-col sm:flex-row justify-around items-center gap-6 text-center">
                 <div>
                    <p class="text-sm text-textMuted mb-1 uppercase tracking-wider">Total Contributions</p>
                    <p class="text-2xl font-bold font-mono text-text">2,143</p>
                    <p class="text-xs text-textMuted mt-1">Jan 1, 2023 - Present</p>
                 </div>
                 <div class="h-12 w-px bg-surfaceHighlight hidden sm:block"></div>
                 <div>
                    <p class="text-sm text-textMuted mb-1 uppercase tracking-wider">Current Streak</p>
                    <p class="text-2xl font-bold font-mono text-warning">12 Days</p>
                    <p class="text-xs text-textMuted mt-1">Jun 25 - Present</p>
                 </div>
                 <div class="h-12 w-px bg-surfaceHighlight hidden sm:block"></div>
                 <div>
                    <p class="text-sm text-textMuted mb-1 uppercase tracking-wider">Longest Streak</p>
                    <p class="text-2xl font-bold font-mono text-text">45 Days</p>
                    <p class="text-xs text-textMuted mt-1">Mar 10 - Apr 24</p>
                 </div>
            </div>
        </section>

        <!-- Current Trajectory Section -->
        <section class="w-full mb-16 animate-fade-in-up" style="animation-delay: 0.6s;">
            <div class="flex items-center justify-center gap-3 mb-8">
                <i class="fa-solid fa-rocket text-error text-2xl"></i>
                <h2 class="text-2xl font-bold text-text">Current Trajectory</h2>
            </div>

            <div class="glass-panel rounded-2xl p-6 sm:p-8 w-full max-w-3xl mx-auto">
                <ul class="space-y-4 text-lg">
                    <li class="flex items-start gap-3">
                        <span class="text-xl mt-1">🔭</span>
                        <p><strong class="text-text">Currently building:</strong> <a href="#" class="text-primary hover:text-secondary transition-colors underline decoration-primary/30 underline-offset-4">Project Name</a> — A high-performance solution for complex data workflows.</p>
                    </li>
                    <li class="flex items-start gap-3">
                        <span class="text-xl mt-1">🌱</span>
                        <p><strong class="text-text">Currently learning:</strong> Advanced Distributed Systems and WebGL rendering techniques.</p>
                    </li>
                    <li class="flex items-start gap-3">
                        <span class="text-xl mt-1">🤝</span>
                        <p><strong class="text-text">Looking to collaborate on:</strong> Impactful Open Source developer tooling and infrastructure projects.</p>
                    </li>
                    <li class="flex items-start gap-3">
                        <span class="text-xl mt-1">💬</span>
                        <p><strong class="text-text">Ask me about:</strong> Frontend architecture, performance optimization, and Developer Experience (DX).</p>
                    </li>
                </ul>
            </div>
        </section>

    </main>

    <!-- Scripts -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const lines = [
                "Hi there, I'm Sharad 👋",
                "Software Engineer & Architect",
                "Building elegant, scalable solutions",
                "Writing code that matters"
            ];
            
            const element = document.getElementById('typewriter-text');
            let currentLineIndex = 0;
            let currentCharIndex = 0;
            let isDeleting = false;
            let typingSpeed = 100;
            
            function type() {
                const currentLine = lines[currentLineIndex];
                
                if (isDeleting) {
                    // Remove char
                    element.textContent = currentLine.substring(0, currentCharIndex - 1);
                    currentCharIndex--;
                    typingSpeed = 50; // Faster when deleting
                } else {
                    // Add char
                    element.textContent = currentLine.substring(0, currentCharIndex + 1);
                    currentCharIndex++;
                    typingSpeed = 100;
                }
                
                // If line is complete
                if (!isDeleting && currentCharIndex === currentLine.length) {
                    typingSpeed = 2000; // Pause at end of line
                    isDeleting = true;
                } else if (isDeleting && currentCharIndex === 0) {
                    isDeleting = false;
                    currentLineIndex = (currentLineIndex + 1) % lines.length; // Move to next line
                    typingSpeed = 500; // Pause before typing next line
                }
                
                setTimeout(type, typingSpeed);
            }
            
            // Start the typing effect
            setTimeout(type, 1000);
        });
    </script>
</body>
</html>
