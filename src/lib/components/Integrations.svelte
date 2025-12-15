<script lang="ts">
    const integrations = [
        { name: 'N8n', color: 'bg-red-500' },
        { name: 'Office 365', color: 'bg-blue-600' },
        { name: 'Google Workspace', color: 'bg-green-500' },
        { name: 'Slack', color: 'bg-purple-500' },
        { name: 'Notion', color: 'bg-white' },
        { name: 'Airtable', color: 'bg-yellow-500' },
        { name: 'Zapier', color: 'bg-orange-500' },
        { name: 'Make', color: 'bg-indigo-500' },
        { name: 'Supabase', color: 'bg-green-600' },
        { name: 'PostgreSQL', color: 'bg-blue-700' },
        { name: 'MongoDB', color: 'bg-green-700' },
        { name: 'OpenAI', color: 'bg-teal-500' },
        { name: 'Anthropic', color: 'bg-orange-400' },
        { name: 'Stripe', color: 'bg-purple-600' },
        { name: 'Twilio', color: 'bg-red-600' },
        { name: 'SendGrid', color: 'bg-blue-400' }
    ];

    const capabilities = [
        'Data lakes', 'Analytics dashboards', 'Monitoring pipelines', 'Automated reporting', 
        'Multi-agent systems', 'Workflow orchestration', 'API integrations', 'Micro-apps', 
        'Privacy-first AI', 'Cost-optimized LLMs', 'Agentic automation', 'Real-time sync'
    ];
</script>

<section class="py-24 bg-black text-white">
	<div class="max-w-[1400px] mx-auto px-6 text-center">
		<h2 class="text-4xl md:text-5xl lg:text-6xl font-serif font-normal mb-6">
			AI-native infrastructure<br />
			built for speed
		</h2>
		<p class="text-gray-400 text-lg max-w-2xl mx-auto mb-20">
			We work with widely adopted platforms and build modular, maintainable solutions designed for rapid iteration.
		</p>

		<div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
            <!-- Integrations -->
			<div>
                <div class="inline-block bg-primary-500 text-white text-[10px] font-bold px-3 py-1 rounded-full mb-8 tracking-wide uppercase">
                    Tools we integrate with
                </div>
                
                <div class="grid grid-cols-4 gap-4">
                    {#each integrations as tool}
                        <div class="aspect-square bg-[#111] rounded-xl border border-white/5 flex flex-col items-center justify-center p-2 hover:bg-[#1a1a1a] transition-colors group">
                            <div class="w-8 h-8 rounded-lg {tool.color} mb-3 flex items-center justify-center opacity-80 group-hover:opacity-100 transition-opacity">
                                <!-- Simple icon placeholder -->
                            </div> 
                            <span class="text-[10px] text-gray-400 font-medium text-center leading-tight">{tool.name}</span>
                        </div>
                    {/each}
                </div>
            </div>

            <!-- Capabilities -->
			<div>
                <div class="inline-block bg-primary-500 text-white text-[10px] font-bold px-3 py-1 rounded-full mb-8 tracking-wide uppercase">
                    Technical capabilities
                </div>
                
                <div class="grid grid-cols-4 gap-4">
                     {#each capabilities as item}
                        <div class="aspect-square bg-[#111] rounded-xl border border-white/5 flex flex-col items-center justify-center p-2 hover:bg-[#1a1a1a] transition-colors group">
                            <div class="w-8 h-8 rounded-full border border-primary-500/30 mb-3 flex items-center justify-center text-primary-400/50 group-hover:text-primary-400 transition-colors">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                    <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"></polyline>
                                </svg>
                            </div> 
                            <span class="text-[10px] text-gray-400 text-center leading-tight font-medium">{item}</span>
                        </div>
                    {/each}
                </div>
            </div>
		</div>
	</div>
</section>
