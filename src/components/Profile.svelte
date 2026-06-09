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

			<div class="flex-1">
				<div class="mb-6 text-center md:text-left">
					<h3 class="text-4xl font-extrabold text-white mb-2 tracking-tight">西住 玄 <span class="text-xl text-slate-400 font-light ml-2">Gen Nishizumi</span></h3>
					<p class="text-cyan-400 font-mono tracking-widest uppercase text-sm">Freelance AI Architect / Paradigm Designer</p>
				</div>

				<div class="space-y-6 text-slate-300 leading-relaxed">
					<p>
						多摩美術大学デザイン科卒業後、東京慈恵会医科大学附属病院にてサーバー管理者としてミッションクリティカルな基盤運用に従事。
					</p>
					<p>
						独立後はフリーランスのAIアーキテクトとして活動。n8nとAIを統合したバックオフィス業務の完全自動化ソリューションの提供や、モダンなWebサービス開発を手掛ける。
					</p>
					<div class="p-6 bg-black/40 border border-slate-800 rounded-lg mt-8 relative overflow-hidden">
						<div class="absolute left-0 top-0 bottom-0 w-1 bg-cyan-500"></div>
						<p class="text-slate-400 italic">
							「美大出身の『デザイン思考』と、医療現場で培った『絶対に止まらないサーバー運用経験』。<br class="hidden sm:block"/>
							この相反する2つのバックグラウンドが、現在の『堅牢かつ洗練されたAIアーキテクチャ』の設計思想の原点となっている。」
						</p>
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
