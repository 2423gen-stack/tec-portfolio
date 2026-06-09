<script>
	export let id = '';
	export let title = '';
	export let subtitle = '';
</script>

<section {id} class="py-24 px-4 relative z-10">
	<div class="max-w-5xl mx-auto">
		<div class="mb-16">
			<h2 class="text-3xl md:text-4xl font-bold tracking-tight text-white mb-4 flex items-center">
				<span class="text-cyan-500 mr-4 font-mono text-xl opacity-70">/</span>
				{title}
			</h2>
			{#if subtitle}
				<p class="text-slate-400 font-light border-l-2 border-cyan-900/50 pl-4">{subtitle}</p>
			{/if}
		</div>
		<slot />
	</div>
</section>
