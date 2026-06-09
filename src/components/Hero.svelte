<script>
	import { onMount } from 'svelte';
	
	let mounted = false;
	
	onMount(() => {
		mounted = true;
	});
</script>

<section class="relative min-h-screen flex flex-col justify-center items-center text-center px-4 overflow-hidden">
	<!-- Abstract Geometric Background Element -->
	<div class="absolute inset-0 z-0 flex justify-center items-center opacity-20 pointer-events-none">
		<div class="w-[800px] h-[800px] border border-cyan-900 rounded-full absolute mix-blend-screen animate-[spin_60s_linear_infinite]"></div>
		<div class="w-[600px] h-[600px] border border-cyan-800 rounded-full absolute mix-blend-screen animate-[spin_40s_linear_infinite_reverse]"></div>
		<div class="w-[400px] h-[400px] border border-cyan-500/30 rounded-full absolute mix-blend-screen animate-[spin_20s_linear_infinite]"></div>
		<div class="absolute w-full h-[1px] bg-cyan-900/50 shadow-[0_0_15px_rgba(0,255,255,0.5)] transform -rotate-45"></div>
		<div class="absolute h-full w-[1px] bg-cyan-900/50 shadow-[0_0_15px_rgba(0,255,255,0.5)] transform -rotate-45"></div>
	</div>

	<div class="z-10 transition-all duration-1000 ease-out transform {mounted ? 'translate-y-0 opacity-100' : 'translate-y-10 opacity-0'}">
		<h2 class="text-cyan-400 font-mono tracking-[0.2em] text-sm md:text-base uppercase mb-6 drop-shadow-[0_0_8px_rgba(0,240,255,0.8)]">
			Gen Nishizumi — AI Architect
		</h2>
		
		<h1 class="text-4xl md:text-6xl lg:text-7xl font-extrabold tracking-tight mb-8 leading-tight">
			If文とSQLを<span class="text-transparent bg-clip-text bg-gradient-to-r from-red-500 to-orange-500">捨てよ。</span><br/>
			<span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-600">多次元幾何学</span>が導く<br/>
			<span class="font-mono bg-slate-900 px-4 py-2 rounded border border-cyan-900/50 inline-block mt-4 shadow-[0_0_20px_rgba(0,255,255,0.15)]">O(1)</span> の制約解決。
		</h1>
		
		<p class="max-w-2xl mx-auto text-slate-400 text-lg md:text-xl font-light leading-relaxed mb-12">
			Discard If-statements and SQL.<br/>
			Achieving O(1) Constraint Resolution through Multi-dimensional Geometry.
		</p>
		
		<p class="max-w-3xl mx-auto text-slate-300 md:text-lg font-normal leading-loose">
			膨大な計算量を強いるレガシーな探索アルゴリズムやリレーショナルデータベースの限界を突破する。<br/>
			AIのセマンティック空間と幾何学処理を融合させた次世代アーキテクチャ「Microforce」の設計と実装。
		</p>
		
		<div class="mt-16 animate-bounce">
			<svg class="w-6 h-6 mx-auto text-cyan-500 opacity-70" fill="none" stroke="currentColor" viewBox="0 0 24 24">
				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
			</svg>
		</div>
	</div>
</section>
