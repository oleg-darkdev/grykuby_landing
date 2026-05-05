<script lang="ts">
	import { navigation, social } from '$sharedData';
	import { AppStoreBtn, PlayStoreBtn } from '$sharedUi';
	import { goto } from '$app/navigation';

	import { scrollToAnchor } from '$sharedUtils';
	// import {  } from '$entities'

	let showNav = $state(false);
</script>

<div id="Hero" class="hero">
	<div class="header">
		<div role="banner" class="navbar">
			<div class=" container">
				<div class="flex w-full flex-row items-center justify-between">
					<a href="#" class="brand flex">
						<img src="images/logo.svg" loading="lazy" width="80" alt="" class="h-10 w-40" />
					</a>
					<div onclick={() => (showNav = !showNav)} class="mobile-only">
						<img src={showNav ? 'images/ovni.svg' : 'images/ovni.svg'} class="h-14 w-14" alt="" />
					</div>
				</div>

				{#if showNav}
					<nav role="navigation" class=" mobile-only flex h-[80vh] flex-col bg-white pt-8">
						{#each navigation as { title, link }}
							<!-- <li class="item_main-nav"> -->
							<div
								onclick={() => {
									showNav = false;
									scrollToAnchor(link);
								}}
								class="nav-link"
							>
								{title}
							</div>
							<!-- </li> -->
							<!-- <div
								class="nav-link my-2"
								on:click|preventDefault={() => {
									scrollToAnchor(link);
								}}
							>
								{title}
							</div> -->
						{/each}

						<div class="mb-4 mt-12 flex flex-col gap-4 px-4 sm:flex-row">
							<PlayStoreBtn />
							<AppStoreBtn />
						</div>

						<div class="mx-4 flex flex-row flex-wrap gap-4 rounded-xl bg-[--blue-violet] px-2 py-4">
							{#each social as { icon, title, link }}
								<a href={link} target="_blank" class="social-link w-inline-block">
									<img src="images/{icon}" loading="lazy" alt={title} />
								</a>
							{/each}
						</div>
					</nav>
				{/if}

				<nav role="navigation" class=" nav-menu desktop-only">
					{#each navigation as { title, link }}
						<a href={link} class="nav-link">{title}</a>
					{/each}
				</nav>
			</div>
		</div>
	</div>

	<div class="hero-elements-absolute">
		<div class="content-hero-section max-width-830 absolute-1">
			<div class="title-section">
				<h1 class="heading-1">INFINITE MINESWEEPER</h1>
			</div>
			<div class="description-section">
				<p class="paragraph">Lorem Ipsum jest tekstem stosowanym jako.</p>
			</div>
			<div class="button-section">
				<div class="button-section">
					<!-- <a href="/" target="_blank" class="button-primary w-button">GET FOR FREE</a> -->
					<div class="my-10 flex w-full flex-col justify-center gap-4 px-4 lg:flex-row">
						<PlayStoreBtn />
						<AppStoreBtn />
					</div>
				</div>
			</div>
		</div>

		<div class="elem-cloud-left">
			<img src="images/cloud-right.svg" loading="lazy" alt="" />
		</div>
		<div class="elem-cloud-center">
			<img src="images/Nube%20center-b.svg" loading="lazy" alt="" />
		</div>
		<div class="elem-cloud-right">
			<img src="images/cloud-right-b.svg" loading="lazy" alt="" />
		</div>

		<div class="elem-circle-blur"></div>
		<div class="elem-ovni">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" />
		</div>
		<div class="elem-pluton-left">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" />
		</div>
		<div class="elem-pluton-right">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" />
		</div>
		<div class="elem-pluton-left-purple">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" />
		</div>

		<div class="elem-rif">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" />
		</div>

		<div class="elem-brain">
			<img src="images/icons/gem_cut.png" loading="lazy" alt="" class="" />
		</div>
		<div class="elem-cloud-white-right"></div>
	</div>
</div>

<style lang="postcss">
	.hero-elements-absolute {
		position: absolute;
		inset: 0%;
		overflow: hidden;
	}

	.content-hero-section.max-width-830 {
		max-width: 830px;
		max-height: 900px;
		margin-left: auto;
		margin-right: auto;
	}

	.content-hero-section.max-width-830.absolute-1 {
		z-index: 11;
		opacity: 1;
		height: 474px;
		margin-top: auto;
		margin-bottom: auto;
		position: absolute;
		inset: 0%;
	}

	.content-hero-section.max-width-830.opacity {
		opacity: 1;
	}

	.content-hero-section.max-width-830.absolute-2 {
		opacity: 1;
		height: 474px;
		margin-top: auto;
		margin-bottom: auto;
		position: absolute;
		inset: 0%;
	}

	@media screen and (max-width: 991px) {
		.nav-menu {
			background-color: #fff;
			width: 100%;
			/* height: 100vh; */
			padding-top: 30vh;
		}

		.content-hero-section.max-width-830.absolute-1,
		.content-hero-section.max-width-830.absolute-2 {
			height: 300px;
			padding-left: 24px;
			padding-right: 24px;
		}
	}
	@media screen and (max-width: 479px) {
		.content-hero-section.max-width-830.absolute-1 {
			top: 0;
		}

		.content-hero-section.max-width-830.absolute-2 {
			display: none;
			top: -20px;
		}
		.nav-menu {
			background-color: #fff;
			background-image: url('/images/cloud-right.svg');
			background-position: -20px 100%;
			background-repeat: no-repeat;
			background-size: 100vh;
			width: 100%;
			/* height: 100vh; */
			padding-top: 30vh;
		}
	}
</style>
