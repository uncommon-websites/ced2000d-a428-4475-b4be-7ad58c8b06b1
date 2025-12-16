<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto bg-[#EAEAE8]">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ PROVEN RESULTS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-8">
			Fly with confidence.
		</h2>
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="m19 9-5 5-4-4-3 3"/></svg>
			View adoption data
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
		<!-- Chart 1 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Pilot Adoption Growth</h3>
			<div class="h-64 relative flex items-end justify-center gap-16 pb-8">
				<!-- Bar 1 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-gray-500 font-mono mb-1 group-hover:text-gray-900">2023</span>
					<div class="w-16 bg-gray-300 rounded-t h-24 relative group-hover:bg-gray-400 transition-colors"></div>
					<span class="font-display text-xl font-medium">2.5K</span>
				</div>
				
				<!-- Bar 2 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-primary-600 font-mono mb-1 font-bold">2024</span>
					<div class="w-16 bg-primary-600 rounded-t h-48 relative group-hover:bg-primary-700 transition-colors">
                        <div class="absolute -top-8 left-1/2 -translate-x-1/2">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor" class="text-primary-600"><path d="M12 2L15 8L21 9L17 14L18 20L12 17L6 20L7 14L3 9L9 8L12 2Z"/></svg>
                        </div>
                    </div>
					<span class="font-display text-xl font-medium text-primary-600">10K+</span>
				</div>
			</div>
		</div>

		<!-- Chart 2 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Response Time vs Traditional Methods</h3>
			<div class="h-64 relative w-full">
                <!-- Simple SVG Line Chart -->
                <svg viewBox="0 0 300 200" class="w-full h-full overflow-visible">
                    <!-- Axes -->
                    <line x1="0" y1="200" x2="300" y2="200" stroke="#ddd" stroke-width="1" />
                    <line x1="0" y1="0" x2="0" y2="200" stroke="#ddd" stroke-width="1" />
                    
                    <!-- Line 1: Manual lookup (Slow) -->
                    <path d="M0,150 Q100,140 150,130 T300,120" fill="none" stroke="#9CA3AF" stroke-width="2" stroke-dasharray="4 4" />
                    <text x="180" y="110" font-family="monospace" font-size="10" fill="#6B7280">Manual Lookup</text>
                    
                    <!-- Line 2: PilotGPT (Fast) -->
                    <path d="M0,190 Q100,188 150,185 T300,180" fill="none" stroke="oklch(0.696 0.17 162.48)" stroke-width="2" />
                    <text x="180" y="170" font-family="monospace" font-size="10" fill="oklch(0.696 0.17 162.48)" font-weight="bold">PILOTGPT</text>
                </svg>
			</div>
            <div class="flex justify-between mt-4 text-[10px] text-gray-400 font-mono uppercase">
                <span>Query Complexity -></span>
                <span>Response Time -></span>
            </div>
		</div>
	</div>
</section>
