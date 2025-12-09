<script>
    import Icon from './Icon.svelte';
    const Sparkles = `<path d="m12 3-1.912 5.813a2 2 0 0 1-1.275 1.275L3 12l5.813 1.912a2 2 0 0 1 1.275 1.275L12 21l1.912-5.813a2 2 0 0 1 1.275-1.275L21 12l-5.813-1.912a2 2 0 0 1-1.275-1.275L12 3Z"/>`;
</script>

<section class="py-24 px-6 relative overflow-hidden">
    <div class="max-w-5xl mx-auto text-center relative z-10">
        <!-- Header -->
        <div class="mb-24">
            <span class="inline-block px-3 py-1 rounded-full bg-white/5 border border-white/10 text-xs font-medium text-gray-400 mb-6">
                The solution
            </span>
            <h2 class="text-4xl md:text-5xl font-bold mb-6">
                Meet Orbi — <span class="text-white/30">your<br/>lead-finding sidekick</span>
            </h2>
            <p class="text-gray-400 max-w-xl mx-auto">
                Orbi scans the internet for new freelance opportunities and drops the best ones into a clean, searchable feed.
            </p>
        </div>

        <!-- Visual Flow -->
        <div class="relative max-w-4xl mx-auto h-[500px] md:h-[400px]">
            
            <!-- Step 1 Card (Left/Back) -->
            <div class="absolute top-10 left-0 md:left-10 w-72 glass-card-darker rounded-xl p-4 transform -rotate-6 z-10 border border-white/10">
                <div class="flex items-center gap-2 mb-4">
                    <div class="w-6 h-6 rounded-full bg-[var(--color-primary)] flex items-center justify-center text-xs font-bold text-white">1</div>
                    <span class="text-sm font-bold text-white">Orbi scans the web</span>
                </div>
                <div class="bg-[#111] rounded-lg p-3 space-y-2">
                    <div class="flex items-center gap-2 text-xs text-white mb-2">
                        <Icon size={12} color="var(--color-primary)">{@html Sparkles}</Icon> Searching for leads
                    </div>
                    <div class="flex items-center gap-2 bg-white/5 p-2 rounded border border-white/5">
                        <div class="w-6 h-6 bg-[#146EF5] rounded flex items-center justify-center text-[8px] font-bold">W</div>
                        <div class="flex-1 h-2 bg-white/10 rounded"></div>
                    </div>
                    <div class="flex items-center gap-2 bg-white/5 p-2 rounded border border-white/5">
                        <div class="w-6 h-6 bg-black rounded flex items-center justify-center text-[8px] font-bold">F</div>
                        <div class="flex-1 h-2 bg-white/10 rounded"></div>
                    </div>
                    <div class="flex items-center gap-2 bg-white/5 p-2 rounded border border-white/5">
                        <div class="w-6 h-6 bg-orange-500 rounded flex items-center justify-center text-[8px] font-bold">L</div>
                        <div class="flex-1 h-2 bg-white/10 rounded"></div>
                    </div>
                </div>
            </div>

            <!-- Arrow 1 -->
             <svg class="absolute top-32 left-64 w-24 h-24 text-gray-600 z-0 hidden md:block" viewBox="0 0 100 100" fill="none">
                <path d="M10 10 C 40 10, 60 40, 80 80" stroke="currentColor" stroke-width="2" stroke-dasharray="4 4"/>
                <path d="M80 80 L 70 75 M 80 80 L 75 70" stroke="currentColor" stroke-width="2"/>
            </svg>

            <!-- Step 2 (Center/Bottom) -->
            <div class="absolute bottom-0 left-1/2 transform -translate-x-1/2 z-20">
                <div class="flex items-center gap-2 bg-black/80 backdrop-blur border border-white/20 px-4 py-2 rounded-full shadow-2xl">
                    <div class="w-6 h-6 rounded-full bg-[var(--color-primary)] flex items-center justify-center text-xs font-bold text-white">2</div>
                    <span class="text-sm font-bold text-white">Rates each lead for quality</span>
                </div>
            </div>

            <!-- Step 3 Card (Right/Front) -->
            <div class="absolute top-0 right-0 md:right-10 w-80 glass-card-darker rounded-xl p-4 transform rotate-3 z-30 border border-white/10 shadow-2xl">
                <div class="flex items-center gap-2 mb-4 justify-end">
                    <span class="text-sm font-bold text-white">Adds it to your feed</span>
                    <div class="w-6 h-6 rounded-full bg-[var(--color-primary)] flex items-center justify-center text-xs font-bold text-white">3</div>
                </div>
                
                <div class="bg-[#111] rounded-lg p-3 space-y-2">
                    <div class="flex justify-between items-center mb-2">
                         <span class="text-xs font-bold text-white"><span class="text-[var(--color-primary)]">34</span> leads found today</span>
                    </div>
                    
                    <!-- Lead Item -->
                    <div class="bg-white/5 p-2 rounded border border-white/5 flex justify-between items-center">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 bg-[#146EF5] rounded flex items-center justify-center text-white text-xs font-bold">W</div>
                            <div>
                                <div class="w-20 h-2 bg-white/20 rounded mb-1"></div>
                                <div class="w-12 h-1.5 bg-white/10 rounded"></div>
                            </div>
                        </div>
                        <div class="bg-green-500/20 text-green-400 text-[8px] font-bold px-1.5 py-0.5 rounded">95% ↑</div>
                    </div>

                    <!-- Lead Item -->
                    <div class="bg-white/5 p-2 rounded border border-white/5 flex justify-between items-center">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 bg-orange-500 rounded flex items-center justify-center text-white text-xs font-bold">L</div>
                            <div>
                                <div class="w-16 h-2 bg-white/20 rounded mb-1"></div>
                                <div class="w-24 h-1.5 bg-white/10 rounded"></div>
                            </div>
                        </div>
                        <div class="bg-green-500/20 text-green-400 text-[8px] font-bold px-1.5 py-0.5 rounded">92% ↑</div>
                    </div>

                    <!-- Lead Item -->
                    <div class="bg-white/5 p-2 rounded border border-white/5 flex justify-between items-center opacity-50">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 bg-gray-700 rounded flex items-center justify-center text-white text-xs font-bold">S</div>
                            <div>
                                <div class="w-20 h-2 bg-white/20 rounded mb-1"></div>
                                <div class="w-10 h-1.5 bg-white/10 rounded"></div>
                            </div>
                        </div>
                         <div class="bg-green-500/20 text-green-400 text-[8px] font-bold px-1.5 py-0.5 rounded">86% ↑</div>
                    </div>
                </div>
            </div>
            
             <!-- Arrow 2 -->
             <svg class="absolute bottom-20 right-64 w-24 h-24 text-gray-600 z-0 hidden md:block transform scale-x-[-1]" viewBox="0 0 100 100" fill="none">
                <path d="M10 10 C 40 10, 60 40, 80 80" stroke="currentColor" stroke-width="2" stroke-dasharray="4 4"/>
                <path d="M80 80 L 70 75 M 80 80 L 75 70" stroke="currentColor" stroke-width="2"/>
            </svg>

        </div>
    </div>
</section>
