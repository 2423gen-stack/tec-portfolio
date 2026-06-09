<script>
	import Section from './Section.svelte';
	
	const tools = [
		{ name: "Python", category: "Core Logic", color: "from-blue-600 to-yellow-500" },
		{ name: "Gemini Advanced Context", category: "LLM Orchestration", color: "from-purple-600 to-blue-500" },
		{ name: "PostgreSQL", category: "Persistence", color: "from-blue-700 to-blue-400" },
		{ name: "Docker", category: "Infrastructure", color: "from-blue-500 to-cyan-400" },
		{ name: "Astro + Svelte", category: "Frontend Representation", color: "from-orange-500 to-red-500" },
		{ name: "Tailwind CSS", category: "Styling", color: "from-cyan-500 to-blue-500" },
		{ name: "n8n + AI", category: "Business Automation", color: "from-pink-500 to-red-500" },
		{ name: "Ubuntu Pro", category: "Base OS", color: "from-orange-600 to-orange-400" },
	];
</script>

<Section 
	id="philosophy" 
	title="Philosophy & Technology Stack" 
>
	<div class="mb-16 relative">
		<div class="absolute -inset-4 bg-gradient-to-r from-cyan-900/20 to-blue-900/20 blur-xl z-0"></div>
		<blockquote class="relative z-10 border-l-4 border-cyan-500 pl-6 py-2 text-xl md:text-2xl font-light text-slate-200 italic leading-relaxed">
			「プログラミング言語やフレームワークは、アーキテクチャを表現するための<span class="text-white font-medium">単なる道具</span>に過ぎない。<br/>
			重要なのは、どのような<span class="text-cyan-400 font-medium">制約を打ち破り</span>、どのような<span class="text-blue-400 font-medium">城を築くか</span>である。」
		</blockquote>
	</div>

	<h3 class="text-xl font-bold text-slate-300 mb-8 font-mono flex items-center">
		<span class="w-8 h-[1px] bg-cyan-900 mr-4"></span>
		CURRENT TOOLKIT
	</h3>

	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
		{#each tools as tool}
			<div class="bg-[#0a0f18] border border-slate-800 rounded-lg p-6 hover:border-slate-600 transition-colors group relative overflow-hidden">
				<div class="absolute inset-0 bg-gradient-to-br {tool.color} opacity-0 group-hover:opacity-10 transition-opacity duration-500"></div>
				<p class="text-xs font-mono text-slate-500 mb-2 uppercase tracking-wider">{tool.category}</p>
				<p class="text-lg font-bold text-slate-200 group-hover:text-white transition-colors">{tool.name}</p>
				<div class="absolute bottom-0 left-0 h-1 w-0 group-hover:w-full bg-gradient-to-r {tool.color} transition-all duration-500"></div>
			</div>
		{/each}
	</div>
</Section>
