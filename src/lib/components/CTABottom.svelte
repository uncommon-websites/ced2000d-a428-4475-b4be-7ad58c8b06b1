<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ READY TO FLY SMARTER? ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Start your free trial today
		</h2>
		<p class="font-mono text-sm text-gray-600">
			Join thousands of pilots flying with confidence using PilotGPT
		</p>
	</div>

	<div class="max-w-4xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
		<div class="bg-[#F3F3F1] p-8 rounded-lg border border-gray-200">
			<form class="space-y-4">
				<div>
					<label for="email" class="block text-[10px] font-mono text-gray-500 uppercase mb-1">Email Address:</label>
					<input type="email" id="email" placeholder="pilot@example.com" class="w-full bg-white border border-gray-200 rounded px-3 py-2 text-sm font-mono text-gray-900 focus:outline-none focus:border-primary-600" />
				</div>
				
				<div>
					<label for="aircraft" class="block text-[10px] font-mono text-gray-500 uppercase mb-1">Aircraft Type (Optional):</label>
					<input type="text" id="aircraft" placeholder="e.g., Cessna 172, Piper Cherokee" class="w-full bg-white border border-gray-200 rounded px-3 py-2 text-sm font-mono text-gray-900 focus:outline-none focus:border-primary-600" />
				</div>
				
				<div>
					<label for="certificate" class="block text-[10px] font-mono text-gray-500 uppercase mb-1">Certificate Level:</label>
					<select id="certificate" class="w-full bg-white border border-gray-200 rounded px-3 py-2 text-sm font-mono text-gray-900 focus:outline-none focus:border-primary-600">
						<option>Student Pilot</option>
						<option>Private Pilot</option>
						<option>Commercial Pilot</option>
						<option>ATP</option>
						<option>CFI</option>
					</select>
				</div>

				<button type="button" class="w-full bg-primary-600 text-white py-3 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center justify-center gap-2 font-mono uppercase tracking-wide">
					<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					Start Free Trial
				</button>
				<p class="text-[10px] text-gray-400 font-mono uppercase text-center">
					No credit card required • Works offline
				</p>
			</form>
            
            <div class="mt-6 pt-6 border-t border-gray-200 text-center">
                <span class="text-xs text-gray-500 font-mono mb-4 block">FLIGHT SCHOOL OR ORGANIZATION?</span>
                <button class="bg-black text-white px-6 py-3 rounded text-sm font-medium hover:bg-gray-800 transition-colors w-full font-mono uppercase tracking-wide">
                    Contact for Group Pricing ->
                </button>
            </div>
		</div>

		<div class="flex items-center justify-center">
			<!-- Cockpit/Device Illustration -->
			<div class="w-full max-w-xs aspect-square bg-gradient-to-br from-primary-100 to-primary-200 border border-gray-200 shadow-lg relative rounded-2xl flex items-center justify-center overflow-hidden">
                <div class="absolute inset-0 opacity-20" 
                    style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 20px 20px;">
                </div>
                <div class="z-10 text-primary-600">
                     <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-32 h-32">
                        <path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
                    </svg>
                </div>
                <div class="absolute bottom-4 left-4 right-4 bg-white/90 backdrop-blur-sm rounded p-3 text-xs font-mono text-gray-700">
                    <div class="font-bold mb-1">✓ Offline Ready</div>
                    <div>Works at any altitude</div>
                </div>
			</div>
		</div>
	</div>
</section>
