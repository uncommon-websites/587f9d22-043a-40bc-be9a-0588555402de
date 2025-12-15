<script lang="ts">
    import { Paperclip, Image, AtSign, Smile, ArrowUp } from 'lucide-svelte';
</script>

<section class="py-24 bg-black text-white">
	<div class="max-w-[1400px] mx-auto px-6">
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
			<div>
				<h2 class="text-4xl md:text-5xl lg:text-6xl font-serif font-normal mb-12 leading-tight">
					Built for founders<br />
					who move fast
				</h2>

				<div class="space-y-6">
					<div class="flex items-center gap-3 text-primary-400 font-medium">
						<div class="w-2 h-2 bg-primary-400 rounded-sm"></div>
						Startups (0-50 employees)
					</div>
					<p class="text-gray-400 text-sm leading-relaxed pl-5 border-l border-white/10 ml-1 mb-8">
						Enterprise-grade execution without the enterprise headcount. Get unified operations, AI infrastructure, and automation in 7-14 days.
					</p>

					<div class="flex items-center gap-3 text-gray-500 hover:text-white transition-colors cursor-pointer">
						<div class="w-2 h-2 bg-gray-500 rounded-sm"></div>
						SMEs (50-500 employees)
					</div>
					<div class="flex items-center gap-3 text-gray-500 hover:text-white transition-colors cursor-pointer">
						<div class="w-2 h-2 bg-gray-500 rounded-sm"></div>
						Legacy companies (500+ employees)
					</div>
					<div class="flex items-center gap-3 text-gray-500 hover:text-white transition-colors cursor-pointer">
						<div class="w-2 h-2 bg-gray-500 rounded-sm"></div>
						Enterprise innovation teams
					</div>
				</div>
			</div>

			<div class="relative">
                <div class="rounded-xl overflow-hidden aspect-square relative bg-gradient-to-br from-gray-900 to-black border border-white/10">
                     <!-- Abstract representation instead of stock photo -->
                     <div class="absolute inset-0 flex items-center justify-center p-12">
                         <div class="w-full h-full relative">
                             <!-- Central node -->
                             <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-24 h-24 rounded-full bg-primary-500/20 border-2 border-primary-500/50 flex items-center justify-center">
                                 <div class="text-primary-400 font-bold text-sm">TBC</div>
                             </div>
                             
                             <!-- Orbiting elements -->
                             <div class="absolute top-12 left-1/2 -translate-x-1/2 w-16 h-16 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
                                 <div class="text-xs text-gray-500">Strategy</div>
                             </div>
                             <div class="absolute bottom-12 left-1/2 -translate-x-1/2 w-16 h-16 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
                                 <div class="text-xs text-gray-500">AI</div>
                             </div>
                             <div class="absolute top-1/2 left-12 -translate-y-1/2 w-16 h-16 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
                                 <div class="text-xs text-gray-500">Process</div>
                             </div>
                             <div class="absolute top-1/2 right-12 -translate-y-1/2 w-16 h-16 rounded-lg bg-white/5 border border-white/10 flex items-center justify-center">
                                 <div class="text-xs text-gray-500">Execute</div>
                             </div>
                             
                             <!-- Connection lines -->
                             <svg class="absolute inset-0 w-full h-full" viewBox="0 0 100 100">
                                 <line x1="50" y1="20" x2="50" y2="40" stroke="oklch(0.696 0.17 162.48)" stroke-width="0.5" stroke-dasharray="2 2" opacity="0.3" />
                                 <line x1="50" y1="60" x2="50" y2="80" stroke="oklch(0.696 0.17 162.48)" stroke-width="0.5" stroke-dasharray="2 2" opacity="0.3" />
                                 <line x1="20" y1="50" x2="40" y2="50" stroke="oklch(0.696 0.17 162.48)" stroke-width="0.5" stroke-dasharray="2 2" opacity="0.3" />
                                 <line x1="60" y1="50" x2="80" y2="50" stroke="oklch(0.696 0.17 162.48)" stroke-width="0.5" stroke-dasharray="2 2" opacity="0.3" />
                             </svg>
                         </div>
                     </div>
                     
                     <!-- Bottom label -->
                     <div class="absolute bottom-8 left-8 right-8 text-center">
                         <div class="text-sm text-gray-400">Unified execution across all domains</div>
                     </div>
                </div>
			</div>
		</div>
	</div>
</section>
