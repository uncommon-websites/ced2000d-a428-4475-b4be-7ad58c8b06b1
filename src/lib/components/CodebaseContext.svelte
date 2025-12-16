<section class="bg-primary-100 py-24 px-6 md:px-12 relative overflow-hidden">
	<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-600 uppercase tracking-widest mb-4 block">
				[ OFFLINE AVIATION AI ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Reliable answers<br>at altitude
			</h2>
			<p class="font-mono text-sm text-gray-700 max-w-md mb-8 leading-relaxed">
				PilotGPT's aviation-trained AI runs entirely on your device. No internet? No problem. Get instant answers to regulations, procedures, and aircraft-specific questions even when you're offline.
			</p>
			
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				Learn about offline mode ->
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Offline indicator visualization -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="relative">
					<!-- Device mockup -->
					<div class="bg-white rounded-2xl shadow-2xl p-6 w-64 border-4 border-gray-800">
						<div class="flex items-center gap-2 mb-4 pb-3 border-b border-gray-200">
							<div class="w-2 h-2 rounded-full bg-gray-300"></div>
							<span class="text-xs font-mono text-gray-400">OFFLINE MODE</span>
						</div>
						<div class="space-y-3">
							<div class="bg-primary-50 p-3 rounded text-xs font-mono">
								<div class="text-gray-600 mb-1">Q: What's my crosswind limit?</div>
								<div class="text-gray-900">A: For Cessna 172S: 15 knots demonstrated...</div>
							</div>
							<div class="bg-gray-50 p-3 rounded">
								<div class="h-2 bg-gray-200 rounded mb-2"></div>
								<div class="h-2 bg-gray-200 rounded w-3/4"></div>
							</div>
						</div>
					</div>
					<!-- Offline badge -->
					<div class="absolute -top-4 -right-4 bg-primary-600 text-white px-3 py-1.5 rounded-full text-xs font-bold shadow-lg">
						✓ OFFLINE
					</div>
				</div>
			</div>
		</div>
	</div>
    
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-10" 
        style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 40px 40px;">
    </div>
</section>
