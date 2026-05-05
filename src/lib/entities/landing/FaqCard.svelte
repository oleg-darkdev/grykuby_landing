<script lang="ts">
	// import {  } from '$shared';
	// import {  } from '$widgets';
	// import {  } from '$entities'

	// console.log(q)

	let { q, a, i } = $props();

	let showAnswer = $state();
</script>

<div class="mb-10">
	<div class="title-section" onclick={(showAnswer = !showAnswer)}>
		<h3 class="text-2xl font-black text-neutral-800 lg:text-4xl">
			<span class="mr-2">{i + 1}.</span>
			{q}
			<!-- <img src="images/icons/gem_cut.png" class="h-10 w-10 bg-black" alt="" /> -->
		</h3>
	</div>
	{#if showAnswer}
		<div class="description-section">
			{#each a as answer}
				<p class="paragraph black">{answer}</p>
			{/each}
		</div>
	{/if}
</div>

<style lang="postcss">
</style>
