<script lang="ts">
    import { Check } from 'lucide-svelte';
</script>

<section class="py-24 bg-black text-white">
	<div class="max-w-[1400px] mx-auto px-6">
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
            <!-- Text Content -->
			<div>
				<h2 class="text-4xl md:text-5xl lg:text-6xl font-serif font-normal mb-6 leading-tight">
					No dependency<br />
					by design
				</h2>
				<p class="text-gray-400 text-lg max-w-md mb-8">
					Every solution is built for maintainability by non-technical users. You own it, you control it, you scale it.
				</p>
				<ul class="space-y-4">
					<li class="flex items-start gap-3">
						<div class="w-5 h-5 rounded-full bg-primary-500 flex items-center justify-center text-white text-[10px] font-bold mt-0.5 shrink-0">✓</div>
						<span class="text-gray-300 text-sm">Complete training and documentation included</span>
					</li>
					<li class="flex items-start gap-3">
						<div class="w-5 h-5 rounded-full bg-primary-500 flex items-center justify-center text-white text-[10px] font-bold mt-0.5 shrink-0">✓</div>
						<span class="text-gray-300 text-sm">Built with widely adopted, stable platforms</span>
					</li>
					<li class="flex items-start gap-3">
						<div class="w-5 h-5 rounded-full bg-primary-500 flex items-center justify-center text-white text-[10px] font-bold mt-0.5 shrink-0">✓</div>
						<span class="text-gray-300 text-sm">Designed for iteration without external support</span>
					</li>
					<li class="flex items-start gap-3">
						<div class="w-5 h-5 rounded-full bg-primary-500 flex items-center justify-center text-white text-[10px] font-bold mt-0.5 shrink-0">✓</div>
						<span class="text-gray-300 text-sm">Full handover ensures client independence</span>
					</li>
				</ul>
			</div>

            <!-- Visual -->
			<div class="bg-[#0f0f0f] rounded-xl p-12 border border-white/5 relative overflow-hidden h-[600px] flex items-center justify-center">
                <div class="w-full h-full flex flex-col items-center justify-center gap-8">
					<!-- Central concept -->
					<div class="w-48 h-48 rounded-2xl bg-primary-500/10 border-2 border-primary-500/30 flex items-center justify-center relative">
						<div class="text-center">
							<div class="text-3xl font-bold text-primary-400 mb-2">You</div>
							<div class="text-xs text-gray-500">Full Control</div>
						</div>
						
						<!-- Radiating elements -->
						<div class="absolute -top-12 left-1/2 -translate-x-1/2 w-20 h-20 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
							<div class="text-[10px] text-gray-500 text-center">Own</div>
						</div>
						<div class="absolute -bottom-12 left-1/2 -translate-x-1/2 w-20 h-20 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
							<div class="text-[10px] text-gray-500 text-center">Maintain</div>
						</div>
						<div class="absolute top-1/2 -translate-y-1/2 -left-24 w-20 h-20 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
							<div class="text-[10px] text-gray-500 text-center">Scale</div>
						</div>
						<div class="absolute top-1/2 -translate-y-1/2 -right-24 w-20 h-20 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
							<div class="text-[10px] text-gray-500 text-center">Iterate</div>
						</div>
					</div>
					
					<div class="text-center text-sm text-gray-500 max-w-xs">
						No vendor lock-in. No ongoing dependency. Just clean, maintainable solutions.
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
