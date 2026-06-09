<script>
	import Section from './Section.svelte';
</script>

<Section 
	id="research" 
	title="Publications & Research" 
	subtitle="ただのエンジニアではなく、パラダイムを創出し世界に問う存在であることを証明する。"
>
	<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
		<!-- Paper 1 -->
		<a href="https://zenodo.org/records/20602701" target="_blank" rel="noopener noreferrer" class="group relative bg-slate-900/40 border border-slate-800 rounded-xl p-8 hover:bg-slate-800/50 hover:border-cyan-500/50 transition-all duration-300 backdrop-blur-sm overflow-hidden flex flex-col h-full">
			<div class="absolute inset-0 bg-gradient-to-br from-cyan-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
			<div class="flex items-center gap-3 mb-4">
				<span class="px-3 py-1 text-xs font-mono text-cyan-300 bg-cyan-900/30 rounded-full border border-cyan-800/50">CERN Zenodo</span>
				<span class="text-slate-500 text-sm font-mono">Paper</span>
			</div>
			<h3 class="text-xl font-bold text-slate-100 mb-3 group-hover:text-cyan-400 transition-colors leading-tight">
				Geometric Resolution Paradigm for NP-Hard Constraints
			</h3>
			<p class="text-slate-400 text-sm leading-relaxed mb-6 flex-grow">
				既存の数理最適化ソルバーが抱える計算量爆発に対し、多次元空間の幾何学的マスク交差により解を O(1) で特定するパラダイムシフト。
			</p>
			<div class="mt-auto flex items-center text-cyan-500 text-sm font-mono group-hover:translate-x-2 transition-transform">
				Read Publication →
			</div>
		</a>

		<!-- Paper 2 -->
		<a href="https://zenodo.org/records/20580181" target="_blank" rel="noopener noreferrer" class="group relative bg-slate-900/40 border border-slate-800 rounded-xl p-8 hover:bg-slate-800/50 hover:border-cyan-500/50 transition-all duration-300 backdrop-blur-sm overflow-hidden flex flex-col h-full">
			<div class="absolute inset-0 bg-gradient-to-br from-cyan-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
			<div class="flex items-center gap-3 mb-4">
				<span class="px-3 py-1 text-xs font-mono text-cyan-300 bg-cyan-900/30 rounded-full border border-cyan-800/50">CERN Zenodo</span>
				<span class="text-slate-500 text-sm font-mono">Paper</span>
			</div>
			<h3 class="text-xl font-bold text-slate-100 mb-3 group-hover:text-cyan-400 transition-colors leading-tight">
				Microforce Constraints Definition Protocol
			</h3>
			<p class="text-slate-400 text-sm leading-relaxed mb-6 flex-grow">
				LLMのセマンティック空間を利用し、業務上の複雑な要件から直接、幾何学エンジンの制約マスクを自動生成・定義するプロトコルの研究。
			</p>
			<div class="mt-auto flex items-center text-cyan-500 text-sm font-mono group-hover:translate-x-2 transition-transform">
				Read Publication →
			</div>
		</a>

		<!-- Article -->
		<a href="https://zenn.dev/unizho/articles/b4b5cd7e53f89a" target="_blank" rel="noopener noreferrer" class="md:col-span-2 group relative bg-slate-900/40 border border-slate-800 rounded-xl p-8 hover:bg-slate-800/50 hover:border-blue-500/50 transition-all duration-300 backdrop-blur-sm overflow-hidden flex flex-col sm:flex-row gap-6 items-start sm:items-center">
			<div class="absolute inset-0 bg-gradient-to-r from-blue-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
			<div class="flex-grow">
				<div class="flex items-center gap-3 mb-4">
					<span class="px-3 py-1 text-xs font-mono text-blue-300 bg-blue-900/30 rounded-full border border-blue-800/50">Zenn / Tech Blog</span>
					<span class="text-slate-500 text-sm font-mono">Article</span>
				</div>
				<h3 class="text-xl md:text-2xl font-bold text-slate-100 mb-3 group-hover:text-blue-400 transition-colors">
					If文とSQLを完全に捨てる — 次世代AI時代のデータ基盤
				</h3>
				<p class="text-slate-400 text-sm md:text-base leading-relaxed">
					既存SQLデータベースベンダーへ向けた技術的アンチテーゼ。手続き型ロジックの廃止と、完全なデータドリブン・幾何学エンジンへの移行記録。
				</p>
			</div>
			<div class="flex-shrink-0 flex items-center justify-center w-12 h-12 rounded-full bg-slate-800 group-hover:bg-blue-900/50 group-hover:text-blue-400 transition-colors">
				<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
			</div>
		</a>
	</div>
</Section>
