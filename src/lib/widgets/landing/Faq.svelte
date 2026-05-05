<script lang="ts">
	import { faq } from '$sharedData';
	// import {  } from '$widgets';
	// import {  } from '$entitiesLanding'

	import { TagsLine, FaqCard } from '$entitiesLanding';
</script>

<section id="faq" class="be-yourself">
	<TagsLine />
	<div class="be-yourself-content">
		<div class="w-container container">
			<div class="content-section">
				<div class="grid-be-yourself">
					<div class="column position-relative"></div>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="w-full">
	<div class="w-container container mx-auto">
		<div class="content-section">
			<h3 class="mx-auto mb-6 text-center text-6xl text-white">F.A.Q.</h3>
			<div class="box-join">
				{#each faq as { q, a }, i}
					<FaqCard {q} {a} {i} />
				{/each}
			</div>
		</div>
	</div>
</section>

<style lang="postcss">
	.content-column.position-relative.slider-cards {
		width: 100%;
		height: 495px;
	}

	.grid-be-yourself {
		grid-column-gap: 55px;
		grid-row-gap: 55px;
		grid-template-rows: auto;
		grid-template-columns: 0.3fr 1fr;
		grid-auto-columns: 1fr;
		display: grid;
	}

	@media screen and (max-width: 991px) {
		.grid-be-yourself {
			grid-template-columns: 1fr;
			padding-left: 40px;
		}
	}

	@media screen and (max-width: 479px) {
		.grid-be-yourself {
			padding-left: 0;
		}
	}
</style>
