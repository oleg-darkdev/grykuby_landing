<script lang="ts">
	// import {  } from '$shared';
	// import {  } from '$widgets';
	// import {  } from '$entities'
	import { AppStoreBtn, PlayStoreBtn } from '$sharedUi';
</script>

<section id='gallery' class="play-fun ">
	<div class="w-container container mx-auto">
		<div class="content-section ">
			<div class="content-box-white">
				<div class="box-white">
					<div class="column visible-mobile">
						<div class="content-column sticky">
							<div class="title-section">
								<h3 class="heading-3">play fun games while you make new friends</h3>
							</div>
							<div class="description-section">
								<p class="paragraph black">
									Został po raz pierwszy użyty w XV w. przez nieznanego drukarza do wypełnienia
									tekstem próbnej książki. Pięć wieków później zaczął być używany przemyśle
									elektronicznym, pozostając praktycznie niezmienionym. Spopularyzował się w latach
									60.
								</p>
							</div>
							<div class="button-section my-10 mb-40 flex flex-col gap-4 px-4 sm:flex-row">
								<PlayStoreBtn />
								<AppStoreBtn />
							</div>
						</div>
					</div>
				</div>
				<div class="grid-2 sticky">
					<div class="column visible-desktop">
						<div class="content-column sticky">
							<div class="title-section">
								<h3 class="heading-3">play fun games while you make new friends</h3>
							</div>
							<div class="description-section">
								<p class="paragraph black">
									Został po raz pierwszy użyty w XV w. przez nieznanego drukarza do wypełnienia
									tekstem próbnej książki. Pięć wieków później zaczął być używany przemyśle
									elektronicznym, pozostając praktycznie niezmienionym. Spopularyzował się w latach
									60.
								</p>
							</div>
							
							<!-- <div class="button-section"> -->
							<!-- <a href="#" class="button-secondary w-button">GET EARLY ACCESS</a> -->
							<!-- </div> -->
						</div>
					</div>
					<div class="column">
						<div class="content-column sticky-2">
							<div class="box-white-mobile"></div>
							<div class="content-box-purple-light">
								<div class="box-purple-light"></div>
								<div class="card-play-4 rounded-xl">
									<img
										src="images/screens/2.png"
										loading="eager"
										sizes="(max-width: 479px) 79vw, (max-width: 991px) 399.52972412109375px, 40vw"
										alt=""
										class="max-card-img"
									/>
								</div>
								<div class="card-play-3">
									<img
										src="images/screens/5.png"
										loading="eager"
										sizes="(max-width: 479px) 74vw, (max-width: 991px) 371.3972473144531px, 37vw"
										alt=""
										class="max-card-img"
									/>
								</div>
								<div class="card-play-2">
									<img
										src="images/screens/10.png"
										loading="eager"
										sizes="(max-width: 479px) 63vw, 320px"
										alt=""
										class="max-card-img"
									/>
								</div>
								<div class="card-play-1">
									<img
										src="images/screens/14.png"
										loading="eager"
										sizes="(max-width: 479px) 63vw, 320px"
										alt=""
										class="max-card-img"
									/>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<style lang="postcss">
	.button-section {
		margin-top: 46px;
	}

	@media screen and (max-width: 991px) {
		.button-section {
			margin: 20px;
		}
	}
</style>
