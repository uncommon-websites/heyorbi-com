<script>
    import Icon from './Icon.svelte';
    
    // Icons
    const Sparkles = `<path d="m12 3-1.912 5.813a2 2 0 0 1-1.275 1.275L3 12l5.813 1.912a2 2 0 0 1 1.275 1.275L12 21l1.912-5.813a2 2 0 0 1 1.275-1.275L21 12l-5.813-1.912a2 2 0 0 1-1.275-1.275L12 3Z"/>`;
    const ArrowRight = `<path d="M5 12h14"/><path d="m12 5 7 7-7 7"/>`;
    const Loader = `<path d="M21 12a9 9 0 1 1-6.219-8.56"/>`;
    
    const XLogo = `<path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/>`;
    const LinkedInLogo = `<path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>`;
    const RedditLogo = `<path d="M12 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0zm5.01 4.744c.688 0 1.25.561 1.25 1.249a1.25 1.25 0 0 1-2.498.056l-2.597-.547-.8 3.747c1.824.07 3.48.632 4.674 1.488.308-.309.73-.491 1.207-.491.968 0 1.754.786 1.754 1.754 1.754 0 .716-.435 1.333-1.01 1.614a3.111 3.111 0 0 1 .042.52c0 2.694-3.13 4.87-7.004 4.87-3.874 0-7.004-2.176-7.004-4.87 0-.183.015-.366.043-.534A1.748 1.748 0 0 1 4.028 12c0-.968.786-1.754 1.754-1.754.463 0 .898.196 1.207.49 1.207-.883 2.878-1.43 4.744-1.487l.885-4.182a.342.342 0 0 1 .14-.197.35.35 0 0 1 .238-.042l2.906.617a1.214 1.214 0 0 1 1.108-.701zM9.25 12C8.561 12 8 12.562 8 13.25c0 .687.561 1.248 1.25 1.248.687 0 1.248-.561 1.248-1.249 0-.688-.561-1.249-1.249-1.249zm5.5 0c-.687 0-1.248.561-1.248 1.25 0 .687.561 1.248 1.249 1.248.688 0 1.249-.561 1.249-1.249 0-.687-.562-1.249-1.25-1.249zm-5.466 3.99a.327.327 0 0 0-.231.094.33.33 0 0 0 0 .463c.842.842 2.484.913 2.961.913.477 0 2.105-.056 2.961-.913a.361.361 0 0 0 .029-.463.33.33 0 0 0-.464 0c-.547.533-1.684.73-2.512.73-.828 0-1.979-.196-2.512-.73a.326.326 0 0 0-.232-.095z"/>`;
</script>

<section class="relative min-h-[90vh] flex flex-col items-center pt-32 pb-20 px-4 overflow-hidden">
    <!-- Background Gradient Mesh -->
    <div class="mesh-gradient">
        <!-- Blue/Cyan top left -->
        <div class="mesh-blob bg-[#00A3FF] w-[600px] h-[600px] -top-[200px] -left-[100px] opacity-40 blur-[100px]"></div>
        <!-- Pink/Purple top center -->
        <div class="mesh-blob bg-[#FF0080] w-[500px] h-[500px] top-[0px] left-[30%] opacity-30 blur-[120px]"></div>
        <!-- Orange/Yellow top right -->
        <div class="mesh-blob bg-[#FF9900] w-[600px] h-[600px] -top-[100px] -right-[100px] opacity-30 blur-[100px]"></div>
        <!-- Bottom right sweep -->
        <div class="mesh-blob bg-[#7928CA] w-[800px] h-[800px] top-[40%] -right-[200px] opacity-20 blur-[150px]"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 text-center max-w-3xl mx-auto mb-16">
        <h1 class="text-5xl md:text-7xl font-bold tracking-tight mb-6 leading-[1.1]">
            <span class="text-white">Your daily list of</span><br/>
            <span class="text-white/40">fresh freelance leads</span>
        </h1>
        <p class="text-lg md:text-xl text-gray-400 mb-10 max-w-2xl mx-auto leading-relaxed">
            Orbi is an agent that <span class="text-white font-medium">finds freelance leads</span> for you. So you can focus on doing great work, not hunting for it.
        </p>

        <!-- Email Form -->
        <div class="flex flex-col items-center gap-3">
            <div class="flex w-full max-w-md bg-[#111] border border-white/10 rounded-xl p-1.5 pl-4 shadow-2xl">
                <input 
                    type="email" 
                    placeholder="Enter your email" 
                    class="bg-transparent border-none outline-none text-white flex-1 placeholder-gray-500 text-sm"
                />
                <button class="bg-[var(--color-primary)] hover:bg-[var(--color-primary-hover)] text-white px-5 py-2.5 rounded-lg text-sm font-medium transition-colors cursor-pointer">
                    Join the beta
                </button>
            </div>
            <p class="text-xs text-gray-600">First 100 sign-ups get a lifetime discount.</p>
        </div>
    </div>

    <!-- Mockup Card -->
    <div class="relative z-10 w-full max-w-md mx-auto perspective-1000">
        <!-- Handwritten Arrow -->
        <div class="absolute -right-[160px] top-[40px] hidden md:block w-40">
            <p class="font-hand text-xl text-white transform -rotate-6 mb-2">Orbi makes finding leads this easy</p>
            <svg width="80" height="60" viewBox="0 0 100 80" fill="none" class="text-white ml-2 transform rotate-12">
                <path d="M80 5 C 60 25, 40 15, 10 55" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"/>
                <path d="M10 55 L 20 50 M 10 55 L 18 63" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"/>
            </svg>
        </div>

        <div class="glass-card rounded-2xl p-6 shadow-2xl border border-white/10 bg-[#111]/80 backdrop-blur-xl">
            <!-- Header -->
            <div class="flex items-center gap-3 mb-6">
                <div class="text-[var(--color-primary)] animate-pulse">
                    <Icon size={24} color="currentColor">{@html Sparkles}</Icon>
                </div>
                <div>
                    <h3 class="text-lg font-semibold text-white">Searching for leads</h3>
                    <p class="text-xs text-gray-500">37 leads found today</p>
                </div>
            </div>

            <!-- List -->
            <div class="space-y-3">
                <!-- Item 1 -->
                <div class="bg-white/5 rounded-xl p-3 flex items-center justify-between border border-white/5 hover:bg-white/10 transition-colors">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-black flex items-center justify-center border border-white/10">
                            <div class="w-5 h-5 text-white">
                                <Icon size={20} fill="currentColor" strokeWidth={0}>{@html XLogo}</Icon>
                            </div>
                        </div>
                        <div>
                            <h4 class="text-sm font-medium text-white">Startup Redesign</h4>
                            <p class="text-xs text-gray-500">Want a cleaner, more modern ...</p>
                        </div>
                    </div>
                    <div class="bg-green-500/20 text-green-400 text-[10px] font-bold px-2 py-1 rounded-full">
                        92% ↑
                    </div>
                </div>

                <!-- Item 2 -->
                <div class="bg-white/5 rounded-xl p-3 flex items-center justify-between border border-white/5 hover:bg-white/10 transition-colors">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#0077B5] flex items-center justify-center">
                            <div class="w-5 h-5 text-white">
                                <Icon size={20} fill="currentColor" strokeWidth={0}>{@html LinkedInLogo}</Icon>
                            </div>
                        </div>
                        <div>
                            <h4 class="text-sm font-medium text-white">Marketing Site Cleanup</h4>
                            <p class="text-xs text-gray-500">Fix spacing, improve load spe...</p>
                        </div>
                    </div>
                    <div class="bg-green-500/20 text-green-400 text-[10px] font-bold px-2 py-1 rounded-full">
                        84% ↑
                    </div>
                </div>

                <!-- Item 3 -->
                <div class="bg-white/5 rounded-xl p-3 flex items-center justify-between border border-white/5 hover:bg-white/10 transition-colors">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#FF4500] flex items-center justify-center">
                            <div class="w-6 h-6 text-white">
                                <Icon size={24} fill="currentColor" strokeWidth={0}>{@html RedditLogo}</Icon>
                            </div>
                        </div>
                        <div>
                            <h4 class="text-sm font-medium text-white">Product Feature Page</h4>
                            <p class="text-xs text-gray-500">Need a standalone page for...</p>
                        </div>
                    </div>
                    <div class="bg-green-500/20 text-green-400 text-[10px] font-bold px-2 py-1 rounded-full">
                        85% ↑
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
