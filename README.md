<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BrandXtra Interactive Sales Playbook</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;700;800&display=swap');
        
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #fafaf9; /* stone-50 */
            color: #1c1917; /* stone-900 */
        }
        
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        
        @media (max-width: 640px) {
            .chart-container {
                height: 250px;
            }
        }

        .tab-btn.active {
            color: #ea580c; /* orange-600 */
            border-bottom: 2px solid #ea580c;
            font-weight: 700;
        }

        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }

        .glass-panel {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(220, 220, 220, 0.5);
        }
    </style>
</head>
<body class="antialiased selection:bg-orange-200 selection:text-orange-900 pb-20">

    <!-- Chosen Palette: Warm Neutrals with Braam Orange/Purple Accents -->
    <!-- Application Structure Plan: A centralized interactive 'Sales Playbook' dashboard. Features a tabbed interface for quick access to outreach scripts, an interactive chart for pricing, and an accordion explorer for the Lead Magnet. The "Our Story" section has been expanded to reflect the founder's mentorship role and agency history. -->

    <header class="bg-white border-b border-stone-200 sticky top-0 z-50">
        <div class="max-w-6xl mx-auto px-6 py-4 flex justify-between items-center">
            <div>
                <h1 class="text-2xl font-extrabold tracking-tight text-stone-900">Brand<span class="text-orange-600">Xtra</span></h1>
                <p class="text-xs uppercase tracking-widest text-stone-500 font-semibold mt-1">Interactive Sales Playbook 2026</p>
            </div>
            <div class="hidden md:flex gap-6 text-sm font-semibold text-stone-600">
                <a href="#about" class="hover:text-orange-600 transition-colors">Our Story</a>
                <a href="#packages" class="hover:text-orange-600 transition-colors">Packages</a>
                <a href="#scripts" class="hover:text-orange-600 transition-colors">Scripts</a>
                <a href="#magnet" class="hover:text-orange-600 transition-colors">Lead Magnet</a>
            </div>
        </div>
    </header>

    <main class="max-w-6xl mx-auto px-6 mt-12 space-y-24">

        <section id="intro" class="text-center max-w-3xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-extrabold mb-6 leading-tight">Convert the Braam Hustle into <span class="text-transparent bg-clip-text bg-gradient-to-r from-orange-600 to-purple-700">Market-Ready Brands.</span></h2>
            <p class="text-lg text-stone-600 leading-relaxed mb-8">
                The pulse of market-ready innovation. This interactive playbook digitizes your outreach, pricing, and growth strategies for the Jozi startup ecosystem.
            </p>
        </section>

        <!-- EXPANDED ABOUT SECTION: THE BRANDXTRA STORY -->
        <section id="about" class="scroll-mt-24">
            <div class="glass-panel border-2 border-orange-100 rounded-3xl p-8 md:p-12 shadow-xl relative overflow-hidden">
                <div class="absolute top-0 right-0 w-32 h-32 bg-orange-100/50 rounded-bl-full -z-10"></div>
                <div class="max-w-4xl">
                    <h3 class="text-sm font-black text-orange-600 uppercase tracking-[0.3em] mb-4 italic">The BX Story</h3>
                    <h4 class="text-3xl font-extrabold text-stone-900 mb-8 leading-tight">From Creative Solutions to <span class="text-orange-600 underline decoration-orange-200 decoration-4">Strategic Mastery.</span></h4>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-stone-700 text-base leading-relaxed">
                        <div class="space-y-4">
                            <p>
                                BrandXtra began as a specialized response to a gap I saw while working in the heart of Johannesburg North's creative hub. As the force behind **Africa Nobuhle Media** and platforms like **The Podcast Cafe** and **Trends Nexus**, I realized that many founders had world-class ideas but lacked the visual and narrative "extra" to secure market trust.
                            </p>
                            <p>
                                My journey as a **Startup Mentor at the Global Entrepreneurship Network (GEN)** revealed a recurring theme: startups weren't failing because of their product—they were failing because their brand didn't look "investor-ready."
                            </p>
                        </div>
                        <div class="space-y-4">
                            <p>
                                We evolved BrandXtra to bridge this gap. By combining content marketing, digital strategy, and media relations, we help entrepreneurs move beyond the "Braamfontein hustle" and into professional market dominance. 
                            </p>
                            <p>
                                Today, we leverage our deep roots in the Jozi ecosystem—from the innovation labs of Tshimologong to the scale-up energy of 22onSloane—to provide elite-level branding that is accessible, impactful, and results-driven.
                            </p>
                        </div>
                    </div>
                    
                    <div class="mt-8 pt-8 border-t border-stone-100 flex flex-wrap gap-4">
                        <div class="flex items-center gap-2 bg-white px-4 py-2 rounded-full border border-stone-200 shadow-sm">
                            <span class="w-2 h-2 bg-orange-600 rounded-full animate-pulse"></span>
                            <span class="text-xs font-bold uppercase tracking-tight text-stone-600">GEN Startup Mentor</span>
                        </div>
                        <div class="flex items-center gap-2 bg-white px-4 py-2 rounded-full border border-stone-200 shadow-sm">
                            <span class="w-2 h-2 bg-purple-600 rounded-full animate-pulse"></span>
                            <span class="text-xs font-bold uppercase tracking-tight text-stone-600">Africa Nobuhle Media</span>
                        </div>
                        <div class="flex items-center gap-2 bg-white px-4 py-2 rounded-full border border-stone-200 shadow-sm">
                            <span class="w-2 h-2 bg-blue-600 rounded-full animate-pulse"></span>
                            <span class="text-xs font-bold uppercase tracking-tight text-stone-600">Jozi Tech Ecosystem</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="packages" class="scroll-mt-24">
            <div class="mb-8">
                <h3 class="text-2xl font-bold text-stone-900 mb-2">&#128202; The BrandXtra Packages</h3>
                <p class="text-stone-600">
                    Understanding the financial trajectory of our clients is crucial. This section visualizes the initial investment required for each tier.
                </p>
            </div>
            
            <div class="glass-panel rounded-2xl p-6 md:p-10 shadow-sm border border-stone-200">
                <div class="chart-container">
                    <canvas id="packageChart"></canvas>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-8">
                    <div class="p-4 border border-orange-200 bg-orange-50 rounded-xl">
                        <div class="font-bold text-orange-800 text-lg mb-1">Braam Launch</div>
                        <div class="text-sm text-orange-600 font-semibold mb-2">R4,500</div>
                        <p class="text-xs text-stone-700 leading-relaxed">Fast visibility for early-stage crews. Basic social setup & identity refresh.</p>
                    </div>
                    <div class="p-4 border border-stone-200 bg-white rounded-xl">
                        <div class="font-bold text-stone-800 text-lg mb-1">Braam Build</div>
                        <div class="text-sm text-stone-600 font-semibold mb-2">R8,500</div>
                        <p class="text-xs text-stone-700 leading-relaxed">Investor-ready identity. Full identity PDF & storytelling package.</p>
                    </div>
                    <div class="p-4 border border-purple-200 bg-purple-50 rounded-xl">
                        <div class="font-bold text-purple-800 text-lg mb-1">Braam Dominate</div>
                        <div class="text-sm text-purple-600 font-semibold mb-2">R12,000 Setup + Retainer</div>
                        <p class="text-xs text-stone-700 leading-relaxed">Full-scale management. Includes advanced storytelling and investor pitch visuals.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="scripts" class="scroll-mt-24">
            <div class="mb-8 max-w-3xl">
                <h3 class="text-2xl font-bold text-stone-900 mb-2">&#128172; Communication Arsenal</h3>
                <p class="text-stone-600">
                    Targeted messaging for LinkedIn, WhatsApp, or Email. Select a channel to view and copy your script.
                </p>
            </div>

            <div class="glass-panel rounded-2xl shadow-sm border border-stone-200 overflow-hidden">
                <div class="flex border-b border-stone-200 bg-stone-100 overflow-x-auto">
                    <button onclick="switchTab('social')" id="tab-social" class="tab-btn active px-6 py-4 text-sm font-semibold text-stone-500 whitespace-nowrap focus:outline-none transition-colors">Social Announcement</button>
                    <button onclick="switchTab('dm')" id="tab-dm" class="tab-btn px-6 py-4 text-sm font-semibold text-stone-500 whitespace-nowrap focus:outline-none transition-colors">Direct Message (DM)</button>
                    <button onclick="switchTab('email')" id="tab-email" class="tab-btn px-6 py-4 text-sm font-semibold text-stone-500 whitespace-nowrap focus:outline-none transition-colors">Email Proposal</button>
                </div>

                <div class="p-6 md:p-8 bg-white relative">
                    <button onclick="copyCurrentScript()" class="absolute top-6 right-6 px-4 py-2 bg-stone-100 hover:bg-orange-100 hover:text-orange-700 text-stone-600 text-xs font-bold uppercase rounded-lg transition-colors border border-stone-200">
                        &#128464; Copy Text
                    </button>
                    <div id="copy-feedback" class="absolute top-6 right-36 text-xs font-bold text-green-600 opacity-0 transition-opacity">Copied!</div>

                    <div id="content-social" class="script-content block">
                        <h4 class="font-bold text-stone-800 mb-4 border-b pb-2 text-xs uppercase tracking-widest">Target: Social Media Announcement</h4>
                        <div class="whitespace-pre-wrap font-mono text-sm text-stone-700 leading-relaxed" id="text-social">From Braam Launch to Market-Ready Brand. 🚀

Braamfontein is the heartbeat of Jozi’s innovation—but is your brand keeping up with your hustle?

Whether you’re a @TshimologongZA prototype, a @22onSloane scale-up, or a creative at Neighbourgoods, your digital presence is your first impression for investors and partners.

We’re officially launching BrandXtra—3 tiered solutions designed specifically for the SA startup ecosystem.

🔥 Starter: Braam Launch (R4,500) - Fast visibility for early-stage crews.
📈 Growth: Braam Build (R8,500) - Investor-ready identity and storytelling.
👑 Pro: Braam Dominate (R7,500/pm) - Full-scale management so you can focus on the product.

PILOT SPECIAL: We are looking for 5 Braam-based innovators to join our pilot phase. Get 20% OFF any package in exchange for a testimonial.

👇 [Link to Digital Brochure]
#BrandXtra #Braamfontein #JoziStartups #AfricaNobuhleMedia</div>
                    </div>

                    <div id="content-dm" class="script-content hidden">
                        <h4 class="font-bold text-stone-800 mb-4 border-b pb-2 text-xs uppercase tracking-widest">Target: LinkedIn / WhatsApp DM</h4>
                        <div class="whitespace-pre-wrap font-mono text-sm text-stone-700 leading-relaxed" id="text-dm">Hi [Name], I’ve been following [Company Name]—love the energy in the Braam space.

I’m currently heading up BrandXtra at Africa Nobuhle Media. We’re helping Jozi startups get 'investor-ready' without the massive agency price tag.

We’re running a pilot for 5 Braam-based companies (20% discount). Even if you're not ready for a kit, let's do a free 10-minute Brand Audit?

Check out our tiers: [Link to Brochure]</div>
                    </div>

                    <div id="content-email" class="script-content hidden">
                        <h4 class="font-bold text-stone-800 mb-4 border-b pb-2 text-xs uppercase tracking-widest">Target: Email Proposal</h4>
                        <div class="whitespace-pre-wrap font-mono text-sm text-stone-700 leading-relaxed" id="text-email">Subject: Proposal: Elevating [Company Name] with BrandXtra

Hi [Founder Name],

It was great connecting. Based on your goal to [mention goal], I recommend the [Package Name] to move you from 'hustle mode' to 'market-ready.'

Why BrandXtra? As a mentor at GEN and lead at Africa Nobuhle Media, I don’t just look at aesthetics—I look at Market Access.

Next Steps:
1. Review the brochure: [Link]
2. Reply 'YES' for the 20% Pilot Discount.
3. We’ll kick off with a strategy call.</div>
                    </div>
                </div>
            </div>
        </section>

        <section id="magnet" class="scroll-mt-24">
            <div class="mb-8">
                <h3 class="text-2xl font-bold text-stone-900 mb-2">&#128218; Lead Magnet: The Free Starter Kit</h3>
                <p class="text-stone-600">
                    Explore the "Braamfontein Brand Audit: 5 Quick Wins for Digital Innovators."
                </p>
            </div>

            <div class="space-y-4">
                <div class="glass-panel border border-stone-200 rounded-xl overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-bold text-stone-800 flex justify-between items-center focus:outline-none hover:bg-stone-50" onclick="toggleAccordion('acc1', this)">
                        Section 1: The Bio Check
                        <span class="text-orange-500 text-xl font-normal transition-transform duration-300 transform">+</span>
                    </button>
                    <div id="acc1" class="accordion-content bg-white">
                        <div class="px-6 py-4 text-stone-600 border-t border-stone-100">
                            Does your IG/LinkedIn bio say what problem you solve, or just what you do? We evaluate the clarity of the value proposition in the critical first 3 seconds.
                        </div>
                    </div>
                </div>

                <div class="glass-panel border border-stone-200 rounded-xl overflow-hidden">
                    <button class="w-full px-6 py-4 text-left font-bold text-stone-800 flex justify-between items-center focus:outline-none hover:bg-stone-50" onclick="toggleAccordion('acc2', this)">
                        Section 2: The Visual Anchor
                        <span class="text-orange-500 text-xl font-normal transition-transform duration-300 transform">+</span>
                    </button>
                    <div id="acc2" class="accordion-content bg-white">
                        <div class="px-6 py-4 text-stone-600 border-t border-stone-100">
                            Why Jozi startups need a consistent color palette to be remembered at networking events.
                        </div>
                    </div>
                </div>

                <div class="bg-gradient-to-r from-orange-600 to-orange-500 text-white border-none rounded-xl overflow-hidden shadow-md mt-6">
                    <div class="px-6 py-6 flex flex-col md:flex-row justify-between items-center">
                        <div class="text-center md:text-left">
                            <div class="font-black uppercase tracking-wider text-xs mb-1 opacity-80 italic">BrandXtra // Pulse of Innovation</div>
                            <div class="font-bold text-lg">"Ready for the 'Extra' in your brand?"</div>
                        </div>
                        <div class="mt-4 md:mt-0 px-4 py-2 bg-white text-orange-600 font-bold rounded-lg text-sm shadow-sm cursor-pointer hover:bg-orange-50 transition-colors">
                            Book Strategy Call
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <footer class="mt-24 border-t border-stone-200 bg-white py-10 text-center">
        <div class="text-stone-400 font-bold text-xl mb-2 tracking-tighter italic">Brand<span class="text-stone-300">Xtra</span></div>
        <p class="text-xs text-stone-500 uppercase tracking-widest font-semibold italic">Powered by Africa Nobuhle Media &copy; 2026</p>
    </footer>

    <textarea id="hidden-clipboard" style="position: absolute; left: -9999px;"></textarea>

    <script>
        const appState = { currentTab: 'social' };

        function switchTab(tabId) {
            appState.currentTab = tabId;
            document.querySelectorAll('.tab-btn').forEach(btn => btn.classList.remove('active'));
            document.querySelectorAll('.script-content').forEach(content => {
                content.classList.remove('block');
                content.classList.add('hidden');
            });
            document.getElementById('tab-' + tabId).classList.add('active');
            const targetContent = document.getElementById('content-' + tabId);
            targetContent.classList.remove('hidden');
            targetContent.classList.add('block');
        }

        function copyCurrentScript() {
            const textElement = document.getElementById('text-' + appState.currentTab);
            const hiddenTextArea = document.getElementById('hidden-clipboard');
            hiddenTextArea.value = textElement.innerText;
            hiddenTextArea.select();
            document.execCommand('copy');
            const feedback = document.getElementById('copy-feedback');
            feedback.style.opacity = '1';
            setTimeout(() => feedback.style.opacity = '0', 2000);
        }

        function toggleAccordion(id, btnElement) {
            const content = document.getElementById(id);
            const icon = btnElement.querySelector('span');
            if (content.style.maxHeight) {
                content.style.maxHeight = null;
                icon.style.transform = "rotate(0deg)";
            } else {
                document.querySelectorAll('.accordion-content').forEach(el => el.style.maxHeight = null);
                document.querySelectorAll('.glass-panel button span').forEach(el => el.style.transform = "rotate(0deg)");
                content.style.maxHeight = content.scrollHeight + "px";
                icon.style.transform = "rotate(45deg)";
            }
        }

        document.addEventListener('DOMContentLoaded', function() {
            const ctx = document.getElementById('packageChart').getContext('2d');
            Chart.defaults.font.family = "'Plus Jakarta Sans', sans-serif";
            new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: ['Braam Launch', 'Braam Build', 'Braam Dominate'],
                    datasets: [{
                        data: [4500, 8500, 12000],
                        backgroundColor: ['#ea580c', '#a8a29e', '#7e22ce'],
                        borderRadius: 8,
                        barPercentage: 0.5
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { legend: { display: false } },
                    scales: {
                        y: { beginAtZero: true, ticks: { callback: v => 'R' + v.toLocaleString() } },
                        x: { grid: { display: false } }
                    }
                }
            });
        });
    </script>
</body>
</html># BX
Interactive sales playbook portal
