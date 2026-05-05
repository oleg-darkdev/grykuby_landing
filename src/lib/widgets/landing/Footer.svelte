<script lang="ts">
	import { social } from '$sharedData';
	import { PlayStoreBtn, AppStoreBtn } from '$sharedUi';
	// import {  } from '$widgets';
	// import {  } from '$entities'
</script>

<footer class="footer">
	<div class="w-container container mx-auto">
		<div class="content-section">
			<div class="flex-elements">
				<div class="">
					<img src="images/logo.svg" loading="lazy" width="80" alt="" class="h-16 w-64" />
				</div>
				<div class="copyright">
					<div>© GryKuby 2023-2026</div>
				</div>
				<div class="flex flex-col items-end">
					<div class="social-icons">
						{#each social as { icon, title, link }}
							<a href={link} target="_blank" class="social-link w-inline-block">
								<img src="{icon}" loading="lazy" alt={title} />
							</a>
						{/each}
					</div>

					<div class="my-4 flex flex-col gap-4  sm:flex-row lg:items-end  w-full">
						<PlayStoreBtn />
						<AppStoreBtn />
					</div>
				</div>
			</div>
		</div>
	</div>
</footer>

<style lang="postcss">
</style>
