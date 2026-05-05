<script lang="ts">
	// import {  } from '$shared';
	// import {  } from '$widgets';
	// import {  } from '$entities'

	let tags = [
		'brain game',
		'time killer',
		'free to play',
		'fun',
		'brain game',
		'time killer',
		'free to play',
		'fun'
		//  thrill  casual
	];
</script>


<div class="mask-repeating-sticky">
		<div class="repeating-line section-1">
			<!--    -->
			<div class="repeting-logo flex flex-row items-center justify-between lg:px-10 px-2">
				{#each tags as tag}
					<h2 class="lg:text-2xl text-lg text-black mr-4"> <span class='-mr-1'>#</span>  {tag}</h2>
					<!-- <img src="/images/icons/gem_cut.png" class=" mx-2 h-10 w-10 bg-black" alt="" /> -->
				{/each}
			</div>
		</div>
	</div>

<style lang="postcss">
</style>
