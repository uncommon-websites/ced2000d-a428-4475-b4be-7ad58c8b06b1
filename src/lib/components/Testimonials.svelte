<script lang="ts">
	const testimonials = [
		{
			quote: "PilotGPT saved my bacon when I couldn't remember the emergency procedure for an alternator failure. Having instant access to aircraft-specific guidance without fumbling through the POH was invaluable.",
			author: "Sarah M.",
			role: "Private Pilot • Cessna 172",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/333/fff?text=C"
		},
		{
			quote: "As a CFI, I was skeptical at first. But PilotGPT's accuracy and offline capability make it a fantastic training tool. My students love having instant answers during ground school.",
			author: "Mike R.",
			role: "CFI • Flight School Owner",
			image: "https://i.pravatar.cc/150?u=mike",
            icon: "https://placehold.co/20x20/000/fff?text=F"
		},
		{
			quote: "The ATC transcription feature is a game-changer. I can review what ATC said after landing and it's helped me improve my radio communication skills tremendously.",
			author: "Jennifer L.",
			role: "Student Pilot • Piper Cherokee",
			image: "https://i.pravatar.cc/150?u=jennifer",
            icon: "https://placehold.co/20x20/purple/fff?text=P"
		},
		{
			quote: "I fly in remote areas where cell service is non-existent. PilotGPT works perfectly offline and has answered questions about weather minimums and airspace that would have otherwise gone unanswered.",
			author: "Tom B.",
			role: "Commercial Pilot • Backcountry",
			image: "https://i.pravatar.cc/150?u=tom",
            icon: "https://placehold.co/20x20/blue/fff?text=B"
		},
		{
			quote: "Finally, an aviation app that understands my specific aircraft. The Cirrus SR22-specific guidance is spot-on and has helped me become a safer pilot.",
			author: "David K.",
			role: "Private Pilot • Cirrus SR22",
			image: "https://i.pravatar.cc/150?u=david",
            icon: "https://placehold.co/20x20/green/fff?text=S"
		},
		{
			quote: "PilotGPT is like having a CFI in your pocket. The instant answers to regulation questions have saved me countless hours of searching through the FAR/AIM.",
			author: "Amanda P.",
			role: "Instrument Student • Diamond DA40",
			image: "https://i.pravatar.cc/150?u=amanda",
            icon: "https://placehold.co/20x20/red/fff?text=D"
		},
        {
			quote: "I've been flying for 30 years and this is the most useful aviation app I've ever used. The offline capability alone makes it worth every penny.",
			author: "Robert H.",
			role: "ATP • Corporate Pilot",
			image: "https://i.pravatar.cc/150?u=robert",
            icon: "https://placehold.co/20x20/333/fff?text=A"
		},
        {
			quote: "Setup took 5 minutes and I was getting accurate answers immediately. The CFI-verified responses give me confidence that I'm getting reliable information.",
			author: "Lisa W.",
			role: "Private Pilot • Beechcraft Bonanza",
			image: "https://i.pravatar.cc/150?u=lisa",
            icon: "https://placehold.co/20x20/orange/fff?text=B"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			From Pilots Who Fly With PilotGPT
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what pilots are saying about their experience with PilotGPT
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
