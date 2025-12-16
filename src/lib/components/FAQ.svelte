<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does PilotGPT work offline?",
			answer: "PilotGPT uses on-device AI that runs entirely on your phone or tablet. Once downloaded, it doesn't require an internet connection to provide answers about regulations, procedures, or aircraft-specific guidance."
		},
		{
			question: "Is PilotGPT FAA-approved?",
			answer: "PilotGPT is a reference tool built with FAA regulations and advisory circulars. While not officially 'approved' by the FAA (as apps don't require approval), all guidance aligns with current FAA standards and is verified by CFIs."
		},
		{
			question: "What aircraft types does PilotGPT support?",
			answer: "PilotGPT supports hundreds of aircraft including popular models like Cessna 172, Piper Cherokee, Cirrus SR20/22, Diamond DA40, Beechcraft Bonanza, and many more. We're constantly adding new aircraft to our database."
		},
		{
			question: "How accurate is the ATC transcription?",
			answer: "Our ATC transcription uses advanced speech recognition trained specifically on aviation communications. Accuracy is typically 90-95% for clear transmissions. The transcription is stored locally on your device for review after your flight."
		},
		{
			question: "Can I use PilotGPT during my checkride?",
			answer: "PilotGPT is a reference tool similar to the FAR/AIM. However, you should check with your DPE about their policy on electronic devices during checkrides. Many pilots use it during the oral portion for quick reference."
		},
		{
			question: "Is there a free trial?",
			answer: "Yes! We offer a 14-day free trial with full access to all features. No credit card required to start."
		},
		{
			question: "Do you offer discounts for flight schools?",
			answer: "Yes, we offer special pricing for flight schools and aviation organizations. Contact us for group pricing details."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-primary-600 transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
