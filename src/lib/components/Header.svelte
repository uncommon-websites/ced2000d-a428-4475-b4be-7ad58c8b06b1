<script lang="ts">
	import { onMount } from 'svelte';
	
	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 20;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 px-6 py-4 flex items-center justify-between {isScrolled ? 'bg-[#EAEAE8]/90 backdrop-blur-md border-b border-gray-200' : 'bg-transparent'}">
	<div class="flex items-center gap-8">
		<a href="/" class="flex items-center gap-2 text-brand-dark font-medium text-xl tracking-tight">
			<div class="w-6 h-6 text-primary-600">
				<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
				</svg>
			</div>
			PilotGPT
		</a>
		
		<nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
			<a href="#features" class="hover:text-gray-900 transition-colors">Features</a>
			<a href="#pricing" class="hover:text-gray-900 transition-colors">Pricing</a>
			<a href="#testimonials" class="hover:text-gray-900 transition-colors">Testimonials</a>
			<a href="#faq" class="hover:text-gray-900 transition-colors">FAQ</a>
		</nav>
	</div>

	<div class="flex items-center gap-4">
		<a href="#signin" class="text-sm font-medium text-white bg-black px-4 py-2 rounded hover:bg-gray-800 transition-colors">Sign In</a>
		<a href="#start" class="text-sm font-medium text-white bg-primary-600 px-4 py-2 rounded hover:bg-primary-700 transition-colors shadow-sm">Get Started</a>
	</div>
</header>
