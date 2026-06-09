<script>
	import Section from './Section.svelte';
</script>

<Section 
	id="profile" 
	title="Profile" 
>
	<div class="relative bg-slate-900/20 border border-slate-800 rounded-2xl p-8 md:p-12 backdrop-blur-sm overflow-hidden">
		<!-- Background geometric accents -->
		<div class="absolute top-0 right-0 w-full h-full opacity-10 pointer-events-none">
			<svg width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
				<defs>
					<pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
						<path d="M 40 0 L 0 0 0 40" fill="none" stroke="currentColor" stroke-width="0.5"/>
					</pattern>
				</defs>
				<rect width="100%" height="100%" fill="url(#grid)" class="text-cyan-500" />
			</svg>
		</div>

		<div class="relative z-10 flex flex-col md:flex-row gap-12 items-center md:items-start">
			<div class="flex-shrink-0 relative">
				<!-- Glitch effect avatar container -->
				<div class="w-48 h-48 rounded-full border-2 border-cyan-500/50 p-2 relative group overflow-hidden">
					<div class="absolute inset-0 bg-cyan-500/20 rounded-full animate-pulse"></div>
					<div class="w-full h-full bg-slate-800 rounded-full flex items-center justify-center relative z-10 border border-slate-700 overflow-hidden">
						<!-- Placeholder for avatar image -->
						<div class="text-5xl font-mono text-slate-600 font-bold group-hover:scale-110 transition-transform duration-500">GN</div>
						<!-- Cyber scanline overlay -->
						<div class="absolute inset-0 bg-[linear-gradient(transparent_50%,rgba(0,0,0,0.25)_50%)] bg-[length:100%_4px] pointer-events-none opacity-50"></div>
					</div>
				</div>
			</div>

			<div class="flex-1 w-full">
				<div class="mb-6 text-center md:text-left">
					<h3 class="text-4xl font-extrabold text-white mb-2 tracking-tight">西住 玄 <span class="text-xl text-slate-400 font-light ml-2">Gen Nishizumi</span></h3>
					<p class="text-cyan-400 font-mono tracking-widest uppercase text-sm">Freelance AI Architect / Paradigm Designer</p>
				</div>

				<div class="space-y-6 text-slate-300 leading-relaxed mb-8">
					<p>
						多摩美術大学デザイン科卒業後、東京慈恵会医科大学附属病院にてサーバー管理者としてミッションクリティカルな基盤運用に従事。
					</p>
					<p>
						独立後はフリーランスのAIアーキテクトとして活動。n8nとAIを統合したバックオフィス業務の完全自動化ソリューションの提供や、モダンなWebサービス開発を手掛ける。
					</p>
					<div class="p-6 bg-black/40 border border-slate-800 rounded-lg relative overflow-hidden">
						<div class="absolute left-0 top-0 bottom-0 w-1 bg-cyan-500"></div>
						<p class="text-slate-400 italic text-sm md:text-base">
							「美大出身の『デザイン思考』と、医療現場で培った『絶対に止まらないサーバー運用経験』。<br class="hidden sm:block"/>
							この相反する2つのバックグラウンドが、現在の『堅牢かつ洗練されたAIアーキテクチャ』の設計思想の原点となっている。」
						</p>
					</div>
				</div>

				<!-- Contact Section -->
				<div class="border-t border-slate-800 pt-6">
					<h4 class="text-slate-400 font-mono text-sm uppercase tracking-wider mb-4 flex items-center gap-2">
						<svg class="w-4 h-4 text-cyan-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
						Contact & Network
					</h4>
					<div class="flex flex-wrap gap-4">
						<a href="mailto:2423gen@gmail.com" class="px-5 py-2 bg-slate-800 hover:bg-cyan-900/40 text-slate-300 hover:text-cyan-400 border border-slate-700 hover:border-cyan-500/50 rounded-lg text-sm font-mono transition-all duration-300 flex items-center gap-2">
							Email
						</a>
						<a href="https://github.com/2423gen-stack" target="_blank" rel="noopener noreferrer" class="px-5 py-2 bg-slate-800 hover:bg-slate-700 text-slate-300 hover:text-white border border-slate-700 rounded-lg text-sm font-mono transition-all duration-300 flex items-center gap-2">
							<svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
							GitHub
						</a>
						<a href="https://zenn.dev/unizho" target="_blank" rel="noopener noreferrer" class="px-5 py-2 bg-slate-800 hover:bg-blue-900/40 text-slate-300 hover:text-blue-400 border border-slate-700 hover:border-blue-500/50 rounded-lg text-sm font-mono transition-all duration-300 flex items-center gap-2">
							Zenn
						</a>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- Footer -->
	<footer class="mt-32 pt-8 border-t border-slate-800 text-center flex flex-col items-center">
		<div class="w-12 h-12 border-t border-l border-cyan-900/50 transform rotate-45 mb-8"></div>
		<p class="text-slate-500 font-mono text-sm">
			© {new Date().getFullYear()} Gen Nishizumi. All Rights Reserved.
		</p>
		<p class="text-slate-600 text-xs mt-2">
			Architected with Astro, Svelte & Tailwind CSS
		</p>
	</footer>
</Section>
