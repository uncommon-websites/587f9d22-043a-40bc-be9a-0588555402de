<script lang="ts">
	import { Menu, X } from 'lucide-svelte';
    import { onMount } from 'svelte';

	let isMenuOpen = false;
    let isScrolled = false;

    function toggleMenu() {
        isMenuOpen = !isMenuOpen;
    }

    onMount(() => {
        const handleScroll = () => {
            isScrolled = window.scrollY > 20;
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });
</script>

<nav class="fixed top-0 left-0 w-full z-50 transition-all duration-300 {isScrolled ? 'bg-black/80 backdrop-blur-md border-b border-white/10' : 'bg-transparent'} text-white">
	<div class="max-w-[1400px] mx-auto px-6 h-20 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="flex items-center gap-3">
			<svg width="32" height="40" viewBox="0 0 90 115" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path fill-rule="evenodd" clip-rule="evenodd" d="M31.8701 9.95388L15.3109 19.4791L31.8819 29.0064L48.446 19.4812L31.8701 9.95388ZM53.2588 27.7795L36.6927 37.3058L36.6911 56.3603L53.2588 46.8319V27.7795ZM58.0696 55.1313L41.5014 64.66L58.072 74.187L74.6383 64.6605L58.0696 55.1313ZM79.4486 72.9601L62.883 82.4862V101.538L79.4486 92.0122V72.9601ZM53.2614 101.539V82.4864L36.6903 72.9591V92.012L53.2614 101.539ZM27.0694 56.3613L10.5003 46.8319V27.7788L27.0711 37.3058L27.0694 56.3613ZM27.0687 67.4269L4.48643 54.4394C2.25391 53.1554 0.878662 50.7828 0.878662 48.215V19.4801C0.878662 17.7684 1.79538 16.1867 3.28356 15.3307L28.2608 0.963381C30.4933 -0.320696 33.2439 -0.321154 35.4766 0.962171L60.474 15.3299C61.963 16.1857 62.8804 17.7679 62.8804 19.4801V46.8319L86.665 60.5111C88.1535 61.3671 89.0702 62.9489 89.0702 64.6607V93.3956C89.0702 95.9635 87.6948 98.3361 85.4621 99.62L60.4776 113.988C58.9894 114.843 57.1558 114.843 55.6673 113.988L30.6773 99.6202C28.4444 98.3365 27.0687 95.9635 27.0687 93.3954V67.4269Z" fill="white"/>
			</svg>
			<span class="text-xl font-bold tracking-tight">TBC Agency</span>
		</a>

		<!-- Desktop Links -->
		<div class="hidden lg:flex items-center gap-8 text-sm font-medium text-gray-300">
			<a href="#framework" class="hover:text-white transition-colors">Framework</a>
			<a href="#outcomes" class="hover:text-white transition-colors">Outcomes</a>
			<a href="#process" class="hover:text-white transition-colors">Process</a>
			<a href="#pricing" class="hover:text-white transition-colors">Pricing</a>
		</div>

		<!-- Right Actions -->
		<div class="hidden lg:flex items-center gap-6">
			<a href="#outcomes" class="text-sm font-medium text-white hover:text-gray-300 transition-colors">See outcomes</a>
			<a href="#workshop" class="bg-primary-500 hover:bg-primary-600 text-white px-5 py-2.5 rounded-full text-sm font-medium transition-colors">
				Run the workshop
			</a>
		</div>

		<!-- Mobile Menu Button -->
		<button class="lg:hidden text-white" onclick={toggleMenu}>
			{#if isMenuOpen}
				<X size={24} />
			{:else}
				<Menu size={24} />
			{/if}
		</button>
	</div>

	<!-- Mobile Menu -->
	{#if isMenuOpen}
		<div class="lg:hidden bg-black absolute top-20 left-0 w-full h-[calc(100vh-80px)] p-6 flex flex-col gap-6 overflow-y-auto border-t border-white/10">
			<a href="#framework" class="text-lg font-medium text-gray-300 hover:text-white">Framework</a>
			<a href="#outcomes" class="text-lg font-medium text-gray-300 hover:text-white">Outcomes</a>
			<a href="#process" class="text-lg font-medium text-gray-300 hover:text-white">Process</a>
			<a href="#pricing" class="text-lg font-medium text-gray-300 hover:text-white">Pricing</a>
			<div class="h-px bg-white/10 my-2"></div>
			<a href="#outcomes" class="text-lg font-medium text-white">See outcomes</a>
			<a href="#workshop" class="bg-primary-500 text-white px-5 py-3 rounded-full text-center font-medium">
				Run the workshop
			</a>
		</div>
	{/if}
</nav>
