<script>
    import Icon from './Icon.svelte';
</script>

<section class="py-24 px-6 relative">
    <div class="max-w-5xl mx-auto">
        <!-- Header -->
        <div class="text-center mb-20">
            <span class="inline-block px-3 py-1 rounded-full bg-white/5 border border-white/10 text-xs font-medium text-gray-400 mb-6">
                The problem
            </span>
            <h2 class="text-4xl md:text-5xl font-bold mb-6">
                Being great <span class="text-white/30">at what<br/>you do</span> isn't enough
            </h2>
            <p class="text-gray-400 max-w-xl mx-auto">
                You're not alone. <span class="text-white">66% of freelancers</span> say lead generation is their #1 problem.
            </p>
        </div>

        <!-- Grid -->
        <div class="space-y-6">
            <!-- Row 1 -->
            <div class="grid md:grid-cols-2 gap-6 bg-[#0A0A0A] border border-white/5 rounded-3xl p-2 items-center">
                <div class="bg-[#111] h-64 rounded-2xl flex items-center justify-center relative overflow-hidden group">
                    <!-- Grid Graphic -->
                    <div class="grid grid-cols-8 gap-2 p-8 opacity-50">
                        {#each Array(32) as _, i}
                            <div class="w-3 h-3 rounded-sm {i === 7 || i === 15 || i === 24 ? 'bg-[var(--color-primary)]' : 'bg-white/10'}"></div>
                        {/each}
                    </div>
                </div>
                <div class="p-8 md:p-12">
                    <h3 class="text-xl font-bold text-white mb-3">Leads are scattered</h3>
                    <p class="text-gray-400 leading-relaxed">
                        Twitter threads, job boards, Reddit posts, funding databases — you're wasting hours just <span class="text-white">finding</span> potential gigs.
                    </p>
                </div>
            </div>

            <!-- Row 2 -->
            <div class="grid md:grid-cols-2 gap-6 bg-[#0A0A0A] border border-white/5 rounded-3xl p-2 items-center">
                <div class="bg-[#111] h-64 rounded-2xl flex items-end justify-center pb-12 gap-3 relative overflow-hidden">
                    <!-- Bar Chart Graphic -->
                    <div class="w-3 h-12 bg-[var(--color-primary)] rounded-t-sm"></div>
                    <div class="w-3 h-6 bg-white/10 rounded-t-sm"></div>
                    <div class="w-3 h-16 bg-[var(--color-primary)] rounded-t-sm"></div>
                    <div class="w-3 h-8 bg-white/10 rounded-t-sm"></div>
                    <div class="w-3 h-4 bg-white/10 rounded-t-sm"></div>
                    <div class="w-3 h-10 bg-white/10 rounded-t-sm"></div>
                    <div class="w-3 h-20 bg-[var(--color-primary)] rounded-t-sm"></div>
                    <div class="w-3 h-14 bg-white/10 rounded-t-sm"></div>
                </div>
                <div class="p-8 md:p-12">
                    <h3 class="text-xl font-bold text-white mb-3">It's inconsistent</h3>
                    <p class="text-gray-400 leading-relaxed">
                        One month you're overloaded. The next, you're refreshing your inbox wondering where everyone went.
                    </p>
                </div>
            </div>

            <!-- Row 3 -->
            <div class="grid md:grid-cols-2 gap-6 bg-[#0A0A0A] border border-white/5 rounded-3xl p-2 items-center">
                <div class="bg-[#111] h-64 rounded-2xl flex items-center justify-center gap-1 relative overflow-hidden px-12">
                    <!-- Flow Graphic -->
                    {#each Array(20) as _, i}
                        <div class="w-1.5 h-32 bg-white/5 rounded-full" style="opacity: {Math.random() * 0.5 + 0.1}"></div>
                    {/each}
                    <div class="absolute inset-0 bg-gradient-to-r from-[#111] via-transparent to-[#111]"></div>
                    <div class="absolute left-12 w-1.5 h-32 bg-[var(--color-primary)]/50 rounded-full blur-sm"></div>
                    <div class="absolute left-16 w-1.5 h-32 bg-[var(--color-primary)] rounded-full"></div>
                </div>
                <div class="p-8 md:p-12">
                    <h3 class="text-xl font-bold text-white mb-3">It kills your creative momentum</h3>
                    <p class="text-gray-400 leading-relaxed">
                        Just when you get in the flow, the outreach grind drags you back.
                    </p>
                </div>
            </div>
        </div>
    </div>
</section>
