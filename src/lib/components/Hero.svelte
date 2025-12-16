<script lang="ts">
	// Aviation organizations
	const partners = [
		{ name: 'AOPA', width: 80 },
		{ name: 'EAA', width: 70 },
		{ name: 'Flight Schools', width: 100 },
		{ name: 'Aviation Safety', width: 90 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Your AI Copilot<br>
				<span class="text-primary-600">In Flight</span>
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Navigation star icon -->
				<svg viewBox="0 0 24 24" fill="none" class="w-10 h-10 text-primary-400 absolute top-0 left-0">
					<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" opacity="0.6"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-700 uppercase tracking-wider leading-relaxed">
					INSTANT AIRCRAFT-SPECIFIC GUIDANCE<br>
					& ATC TRANSCRIPTION VIA OFFLINE<br>
					AVIATION-TRAINED AI
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-primary-600 text-white px-6 py-3 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2">
						Start Free Trial
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						Works offline - no internet required in flight
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center" id="hero-image">
			<!-- Hero image -->
			<div class="absolute inset-0 flex items-center justify-center">
				<img src="/generated/image-a-private-pilot-in-a-small-aircraft-cock-1765844854526-0.webp" alt="Pilot using PilotGPT in cockpit" class="w-full h-full object-cover rounded-lg shadow-2xl" />
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			Trusted by 600K+ certificated pilots nationwide
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-4 gap-8 opacity-60 grayscale">
			{#each partners as partner}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{partner.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
