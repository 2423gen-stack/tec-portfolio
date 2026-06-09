<script>
	import Section from './Section.svelte';
</script>

<Section 
	id="architectures" 
	title="Architectures & Deliverables" 
	subtitle="理論だけでなく、実際に稼働するプロダクト・エンジンを持っていることの証明。"
>
	<div class="space-y-8">
		<!-- Core Engine -->
		<div class="relative bg-[#080c14] border border-[#1a2333] rounded-2xl p-8 overflow-hidden group">
			<div class="absolute top-0 right-0 w-64 h-64 bg-cyan-900/10 rounded-full blur-3xl -mr-20 -mt-20 pointer-events-none"></div>
			
			<div class="flex flex-col lg:flex-row justify-between gap-8 items-start lg:items-center relative z-10">
				<div class="flex-1">
					<div class="flex items-center gap-3 mb-4">
						<div class="w-2 h-2 rounded-full bg-cyan-500 animate-pulse"></div>
						<span class="text-slate-400 font-mono text-sm tracking-wider uppercase">Core Engine</span>
					</div>
					<h3 class="text-3xl font-extrabold text-white mb-4 tracking-tight">Microforce</h3>
					<p class="text-slate-300 leading-relaxed max-w-2xl text-lg">
						NP困難な制約充足問題を、多次元テンソル（幾何学）処理により瞬時に解決する独自エンジン。<br/>
						膨大なループ処理を排除し、O(1)的な挙動で最適解を導出する。
					</p>
				</div>
				
				<div class="flex-shrink-0 flex flex-col sm:flex-row gap-4 w-full lg:w-auto">
					<a href="https://github.com/2423gen-stack/microforce-core" target="_blank" rel="noopener noreferrer" class="flex items-center justify-center gap-2 px-6 py-3 bg-slate-800 hover:bg-slate-700 text-white rounded-lg transition-colors font-mono text-sm border border-slate-700">
						<svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
						Core Repository
					</a>
				</div>
			</div>
			
			<!-- Visual abstract representation of Microforce engine -->
			<div class="mt-8 pt-8 border-t border-slate-800/50 flex flex-wrap gap-3">
				<span class="px-3 py-1 bg-black border border-slate-800 rounded text-xs font-mono text-slate-400">Tensor Math</span>
				<span class="px-3 py-1 bg-black border border-slate-800 rounded text-xs font-mono text-slate-400">Geometric Intersection</span>
				<span class="px-3 py-1 bg-black border border-slate-800 rounded text-xs font-mono text-slate-400">Constraint Satisfaction</span>
				<span class="px-3 py-1 bg-black border border-slate-800 rounded text-xs font-mono text-slate-400">O(1) Resolution</span>
			</div>
		</div>

		<!-- Live Demo -->
		<div class="relative bg-gradient-to-br from-slate-900 to-[#030a14] border border-cyan-900/30 rounded-2xl p-8 overflow-hidden group hover:border-cyan-500/50 transition-colors">
			<div class="absolute bottom-0 left-0 w-full h-1 bg-gradient-to-r from-transparent via-cyan-500 to-transparent opacity-30 group-hover:opacity-100 transition-opacity"></div>
			
			<div class="flex flex-col lg:flex-row justify-between gap-8 items-start lg:items-center relative z-10">
				<div class="flex-1">
					<div class="flex items-center gap-3 mb-4">
						<span class="relative flex h-3 w-3">
						  <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
						  <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
						</span>
						<span class="text-green-400 font-mono text-sm tracking-wider uppercase">Live Production</span>
					</div>
					<h3 class="text-2xl md:text-3xl font-bold text-white mb-4">Autonomous Shift Scheduler</h3>
					<p class="text-slate-300 leading-relaxed max-w-2xl">
						Microforceエンジンを基盤に構築された実稼働シフト自動作成システム。<br/>
						複雑な人間関係や労働条件の制約を幾何学的に解決し、瞬時に最適スケジュールを生成。
					</p>
				</div>
				
				<div class="flex-shrink-0 flex flex-col sm:flex-row gap-4 w-full lg:w-auto">
					<a href="https://github.com/2423gen-stack/microforce-shift" target="_blank" rel="noopener noreferrer" class="flex items-center justify-center gap-2 px-6 py-3 bg-slate-800/80 hover:bg-slate-700 text-white rounded-lg transition-colors font-mono text-sm border border-slate-700">
						<svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
						Source Code
					</a>
					<a href="https://shift.okyn.net" target="_blank" rel="noopener noreferrer" class="flex items-center justify-center gap-2 px-6 py-3 bg-cyan-600/20 hover:bg-cyan-500/30 text-cyan-300 rounded-lg transition-colors font-mono text-sm border border-cyan-500/50 shadow-[0_0_15px_rgba(0,255,255,0.1)]">
						Launch Demo
						<svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"></path></svg>
					</a>
				</div>
			</div>
		</div>
	</div>
</Section>
