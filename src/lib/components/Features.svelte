<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FLY WITH CONFIDENCE ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Aviation AI that works<br>when you need it most.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				PilotGPT delivers instant answers and ATC transcription, even without internet connection.
			</p>
		</div>
		
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			See PilotGPT in action ->
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ OFFLINE CAPABLE ]"
			title="Works without<br>internet connection"
			description="Aviation-trained AI runs locally on your device. Get answers even at 10,000 feet."
			tagColor="bg-primary-600"
			tagIcon="arrow"
            imageSrc="/generated/image-close-up-of-a-pilots-hand-holding-a-smar-1765844857269-1.webp"
		/>
		
		<FeatureCard 
			subtitle="[ ATC TRANSCRIPTION ]"
			title="Real-time ATC<br>transcription & playback"
			description="Never miss a clearance. PilotGPT transcribes and stores all ATC communications."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="/generated/image-interior-view-of-a-cessna-172-cockpit-wi-1765844864507-4.webp"
		/>
		
		<FeatureCard 
			subtitle="[ AIRCRAFT-SPECIFIC ]"
			title="Guidance tailored to<br>your aircraft"
			description="Get answers specific to your aircraft's systems, limitations, and procedures."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="/generated/image-interior-view-of-a-cessna-172-cockpit-wi-1765844864507-4.webp"
		/>
		
		<FeatureCard 
			subtitle="[ CFI ENDORSED ]"
			title="Trusted by certified<br>flight instructors"
			description="Built with input from CFIs and tested by aviation professionals for accuracy."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="/generated/image-a-certified-flight-instructor-cfi-teachi-1765844859624-2.webp"
		/>
	</div>
</section>
