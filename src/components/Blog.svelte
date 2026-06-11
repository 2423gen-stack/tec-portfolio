<script>
	import Section from './Section.svelte';
	
	const articles = [
		{
			title: "MicroforceDBの原点",
			date: "2026.06.11",
			description: "AIチャットから閃いた多次元幾何学処理DB。RDBMSを廃し、多次元幾何学とトポロジーで推論を解くSemantic KVSの実装録。",
			url: "/articles/microforce-db-prototype",
			thumbnail: "/images/microforce-db-prototype.webp"
		}
	];
</script>

<Section 
	id="blog" 
	title="Latest Articles" 
	subtitle="思考の結晶化と、アーキテクチャの探求の記録。"
>
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
		{#each articles as article}
			<a href={article.url} class="group block relative bg-[#080c14] border border-[#1a2333] hover:border-cyan-500/50 rounded-2xl overflow-hidden transition-all duration-300 hover:-translate-y-1 hover:shadow-[0_10px_30px_-15px_rgba(0,255,255,0.2)]">
				<div class="aspect-video overflow-hidden bg-slate-900 border-b border-[#1a2333]">
					{#if article.thumbnail}
						<img src={article.thumbnail} alt={article.title} class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" loading="lazy" />
					{:else}
						<div class="w-full h-full bg-gradient-to-br from-slate-800 to-slate-900 flex items-center justify-center">
							<svg class="w-12 h-12 text-slate-700" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M19 20H5a2 2 0 01-2-2V6a2 2 0 012-2h10a2 2 0 012 2v1m2 13a2 2 0 01-2-2V7m2 13a2 2 0 002-2V9.5L18.5 7H20"></path></svg>
						</div>
					{/if}
				</div>
				<div class="p-6 relative">
					<div class="absolute top-0 right-0 w-24 h-24 bg-cyan-900/10 rounded-full blur-2xl -mr-10 -mt-10 pointer-events-none group-hover:bg-cyan-500/20 transition-colors duration-500"></div>
					<div class="flex items-center gap-3 mb-3">
						<span class="text-cyan-400 font-mono text-xs tracking-wider">{article.date}</span>
					</div>
					<h3 class="text-xl font-bold text-white mb-3 group-hover:text-cyan-300 transition-colors">{article.title}</h3>
					<p class="text-slate-400 text-sm leading-relaxed line-clamp-3">
						{article.description}
					</p>
				</div>
			</a>
		{/each}
	</div>
</Section>
