<script>
    import Icon from './Icon.svelte';
</script>

<nav class="absolute top-0 left-0 w-full z-50 px-6 py-6 flex justify-between items-center max-w-7xl mx-auto left-0 right-0">
    <div class="flex items-center gap-2">
        <!-- Logo Icon -->
        <div class="w-8 h-8 bg-white rounded-lg flex items-center justify-center transform rotate-12">
            <div class="w-4 h-4 bg-black rounded-full"></div>
        </div>
    </div>

    <a href="#beta" class="bg-[rgba(255,255,255,0.1)] hover:bg-[rgba(255,255,255,0.15)] text-white px-4 py-2 rounded-lg text-sm font-medium transition-colors border border-white/5">
        Join the beta
    </a>
</nav>
