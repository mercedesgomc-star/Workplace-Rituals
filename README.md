# Workplace-Rituals
Practices to help you destress at your workspace. 
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Workplace Tools | Holistic Stress Regulation</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,500;1,400&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'yoga-beige': '#F2EFE9',
                        'yoga-green': '#2E4733',
                        'yoga-brown': '#8A5A44',
                        'yoga-light': '#FAFAF8',
                    },
                    fontFamily: {
                        'serif': ['Lora', 'serif'],
                        'sans': ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #F2EFE9;
            color: #2E4733;
        }
        
        /* Fade-in animation classes */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Breathing circle animation */
        .breathe-circle {
            transition: transform 4s linear, background-color 4s ease;
        }
        .inhale {
            transform: scale(1.6);
            background-color: #2E4733; /* Deep green */
        }
        .hold-inhale {
            transform: scale(1.6);
            background-color: #3f6146; 
        }
        .exhale {
            transform: scale(1);
            background-color: #8A5A44; /* Warm brown */
        }
        .hold-exhale {
            transform: scale(1);
            background-color: #6b4432;
        }
    </style>
</head>
<body class="font-sans antialiased text-lg leading-relaxed">

    <header class="min-h-[85vh] flex flex-col items-center justify-center text-center px-6 relative">
        <div class="fade-in max-w-2xl mx-auto">
            <span class="text-yoga-brown font-medium tracking-widest uppercase text-sm mb-4 block">Holistic Workplace Tools</span>
            <h1 class="font-serif text-5xl md:text-6xl text-yoga-green mb-6 leading-tight">Pause.<br>Breathe.<br>Reconnect.</h1>
            <p class="text-yoga-green/80 font-light text-lg md:text-xl max-w-md mx-auto mt-4">
                Practical, yogic techniques to regulate your nervous system and release tension during your workday.
            </p>
        </div>
        <div class="absolute bottom-10 animate-bounce text-yoga-green/50">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3" />
            </svg>
        </div>
    </header>

    <section class="py-20 px-6 bg-yoga-light">
        <div class="max-w-3xl mx-auto fade-in">
            <h2 class="font-serif text-3xl md:text-4xl text-yoga-green mb-6 text-center">Your Body is Your Anchor</h2>
            <p class="text-yoga-green/80 mb-6 text-center">
                The modern workday keeps our energy concentrated in our minds, often leading to a state of chronic low-level stress. By shifting our attention back to the physical body, we can signal safety to our nervous system. 
            </p>
            <p class="text-yoga-green/80 text-center">
                Use these three minimalistic tools anywhere, anytime to reset your focus and cultivate inner calm.
            </p>
        </div>
    </section>

    <section class="py-24 px-6 relative overflow-hidden">
        <div class="max-w-xl mx-auto fade-in">
            <div class="text-center mb-12">
                <span class="text-yoga-brown font-medium tracking-widest uppercase text-xs">Tool 01</span>
                <h2 class="font-serif text-3xl md:text-4xl mt-2 mb-4">Box Breathing</h2>
                <p class="text-yoga-green/80 text-base">A powerful technique to clear the mind, relax the body, and improve focus. Follow the circle below.</p>
            </div>

            <!-- Interactive Breathing Visualizer -->
            <div class="bg-yoga-light rounded-3xl p-8 shadow-[0_8px_30px_rgb(0,0,0,0.04)] flex flex-col items-center justify-center min-h-[350px]">
                <div class="relative w-24 h-24 mb-12 flex items-center justify-center">
                    <div id="breath-circle" class="absolute w-full h-full rounded-full bg-yoga-brown opacity-20 breathe-circle"></div>
                    <div class="absolute w-4 h-4 rounded-full bg-yoga-green z-10"></div>
                </div>
                <div id="breath-text" class="font-serif text-2xl text-yoga-green mb-2 h-8 transition-opacity duration-500">Ready?</div>
                <div class="text-yoga-brown/80 text-sm h-6">
                    <span id="breath-timer" class="font-mono">4.0</span>s
                </div>
                
                <button id="start-breath-btn" class="mt-8 px-6 py-2 rounded-full border border-yoga-green text-yoga-green hover:bg-yoga-green hover:text-yoga-beige transition-colors duration-300 text-sm tracking-wide uppercase">
                    Start Exercise
                </button>
            </div>
        </div>
    </section>

    <section class="py-24 px-6 bg-yoga-light">
        <div class="max-w-xl mx-auto fade-in">
            <div class="text-center mb-10">
                <span class="text-yoga-brown font-medium tracking-widest uppercase text-xs">Tool 02</span>
                <h2 class="font-serif text-3xl md:text-4xl mt-2 mb-4">The Body Shake</h2>
                <p class="text-yoga-green/80 text-base">Animals instinctively shake their bodies to discharge stress hormones after a threat. We can do the same.</p>
            </div>

            <div class="space-y-6 text-yoga-green/90 text-base">
                <div class="flex items-start">
                    <div class="flex-shrink-0 w-8 h-8 rounded-full border border-yoga-brown flex items-center justify-center text-yoga-brown mr-4 mt-1">1</div>
                    <p><strong>Stand up</strong> and find a quiet space. Let your arms hang loose at your sides.</p>
                </div>
                <div class="flex items-start">
                    <div class="flex-shrink-0 w-8 h-8 rounded-full border border-yoga-brown flex items-center justify-center text-yoga-brown mr-4 mt-1">2</div>
                    <p><strong>Start small:</strong> Shake your hands from the wrists, as if shaking off water. Let the movement travel up to your elbows and shoulders.</p>
                </div>
                <div class="flex items-start">
                    <div class="flex-shrink-0 w-8 h-8 rounded-full border border-yoga-brown flex items-center justify-center text-yoga-brown mr-4 mt-1">3</div>
                    <p><strong>Involve the whole body:</strong> Gently bounce on your heels, allowing the vibration to move through your spine, hips, and legs. Let out a sigh as you exhale.</p>
                </div>
                <div class="flex items-start">
                    <div class="flex-shrink-0 w-8 h-8 rounded-full border border-yoga-brown flex items-center justify-center text-yoga-brown mr-4 mt-1">4</div>
                    <p><strong>Pause and feel:</strong> Stop after 60 seconds. Stand still, close your eyes, and notice the tingling sensation and renewed blood flow.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="py-24 px-6">
        <div class="max-w-xl mx-auto fade-in">
            <div class="text-center mb-10">
                <span class="text-yoga-brown font-medium tracking-widest uppercase text-xs">Tool 03</span>
                <h2 class="font-serif text-3xl md:text-4xl mt-2 mb-4">Body Tapping</h2>
                <p class="text-yoga-green/80 text-base">Rooted in ancient Eastern practices, tapping stimulates meridians to release stagnant energy and ground the mind.</p>
            </div>

            <div class="bg-white/40 backdrop-blur-sm rounded-3xl p-8 border border-yoga-green/10">
                <ul class="space-y-5 text-yoga-green/90 text-base">
                    <li class="flex items-center">
                        <svg class="w-5 h-5 text-yoga-brown mr-3" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                        <strong>The Chest:</strong> Use your fingertips to tap firmly but gently on your upper chest, right below the collarbones. Breathe deeply.
                    </li>
                    <li class="flex items-center">
                        <svg class="w-5 h-5 text-yoga-brown mr-3" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                        <strong>The Arms:</strong> Cup your hand slightly and tap down the outside of one arm, and up the inside. Repeat on the other side.
                    </li>
                    <li class="flex items-center">
                        <svg class="w-5 h-5 text-yoga-brown mr-3" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                        <strong>The Legs:</strong> While seated, tap down the outside of your thighs and calves, and back up the inner legs.
                    </li>
                    <li class="flex items-center">
                        <svg class="w-5 h-5 text-yoga-brown mr-3" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                        <strong>The intention:</strong> Imagine waking up the nervous system and brushing off accumulated stress.
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <footer class="py-12 px-6 bg-yoga-green text-yoga-beige text-center">
        <div class="max-w-md mx-auto">
            <h3 class="font-serif text-2xl mb-4 text-yoga-beige">Return to your center.</h3>
            <p class="font-light text-sm opacity-70 mb-8">Take these tools with you throughout your day. You hold the key to your own equilibrium.</p>
            <div class="text-xs opacity-50 border-t border-yoga-beige/20 pt-6">
                © Holistic Workspace Wellbeing
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach((entry) => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, { threshold: 0.1 });

            document.querySelectorAll('.fade-in').forEach((el) => {
                observer.observe(el);
            });

            const btn = document.getElementById('start-breath-btn');
            const circle = document.getElementById('breath-circle');
            const textElement = document.getElementById('breath-text');
            const timerElement = document.getElementById('breath-timer');
            
            let isBreathing = false;
            let breathingInterval;
            let timerInterval;

            const phases = [
                { text: 'Inhale...', class: 'inhale' },
                { text: 'Hold...', class: 'hold-inhale' },
                { text: 'Exhale...', class: 'exhale' },
                { text: 'Hold...', class: 'hold-exhale' }
            ];

            function runBreathingCycle() {
                let currentPhase = 0;
                let phaseTime = 4000; // 4 seconds per phase
                let startTime = Date.now();

                function updatePhase() {
                    // Remove previous classes
                    phases.forEach(p => circle.classList.remove(p.class));
                    
                    // Add current class and text
                    circle.classList.add(phases[currentPhase].class);
                    textElement.style.opacity = 0;
                    
                    setTimeout(() => {
                        textElement.innerText = phases[currentPhase].text;
                        textElement.style.opacity = 1;
                    }, 200);

                    startTime = Date.now();
                    currentPhase = (currentPhase + 1) % 4;
                }

                // Initial trigger
                updatePhase();
                
                // Interval for phases
                breathingInterval = setInterval(updatePhase, phaseTime);

                // Interval for timer update (smooth countdown)
                timerInterval = setInterval(() => {
                    let elapsed = Date.now() - startTime;
                    let remaining = Math.max(0, (phaseTime - elapsed) / 1000).toFixed(1);
                    timerElement.innerText = remaining;
                }, 100);
            }

            btn.addEventListener('click', () => {
                if (isBreathing) {
                    // Stop breathing
                    clearInterval(breathingInterval);
                    clearInterval(timerInterval);
                    phases.forEach(p => circle.classList.remove(p.class));
                    textElement.innerText = 'Ready?';
                    timerElement.innerText = '4.0';
                    btn.innerText = 'Start Exercise';
                    isBreathing = false;
                } else {
                    // Start breathing
                    btn.innerText = 'Stop Exercise';
                    isBreathing = true;
                    runBreathingCycle();
                }
            });
        });
    </script>
</body>
</html>
