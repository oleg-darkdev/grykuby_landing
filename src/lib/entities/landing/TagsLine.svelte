<script lang="ts">
	import { tags } from '$sharedData';
	// import {  } from '$widgets';
	// import {  } from '$entities'
</script>

<div class="mask-repeating-sticky">
	<div class="repeating-line section-1">
		<!--    -->
		<div class="repeting-logo flex flex-row items-center justify-between px-2 lg:px-10">
			{#each tags as tag}
				<h2 class="mr-4 text-lg text-black lg:text-2xl"><span class="-mr-1">#</span> {tag}</h2>
				<!-- <img src="/images/icons/gem_cut.png" class=" mx-2 h-10 w-10 bg-black" alt="" /> -->
			{/each}
		</div>
	</div>
</div>

<style lang="postcss">
</style>
