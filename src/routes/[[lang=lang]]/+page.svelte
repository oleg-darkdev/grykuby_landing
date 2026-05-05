<script lang="ts">
	import {} from '$sharedData';
	import {} from '$sharedUi';
	import { Hero, Features, Footer, Cta, Gallery, Faq } from '$widgetsLanding';
	// import { SEO } from '$sharedUtils';
</script>

<svelte:head>
	<title>GryKuby | Home</title>
	<meta name="description" content="" />
</svelte:head>

<!-- <SEO title="Home" /> -->

<div style="" class="modal-waitlist">
	<div class="join-the-waitlist position-relative">
		<div class="overlay-modal"></div>
		<div class="position-relative m-box-join w-container container">
			<div class="content-section">
				<!-- <div class="box-join">
					<div class="title-section">
						<div class="letter-animation">
							<h3 class="split-text is--large">JOIN THE WAITLIST</h3>
						</div>
					</div>
					<div class="description-section">
						<p class="paragraph black">Get exclusive access first.</p>
					</div>
					<div class="form-section">
						<div class="w-form">
							<form id="email-form" name="email-form">
								<input
									class="text-field w-input"
									maxlength="256"
									name="Email-bottom-2"
									placeholder="YOUR EMAIL"
									type="email"
									id="Email-bottom-2"
									required=""
								/>
								<input
									type="submit"
									data-wait="Please wait..."
									class="submit-button w-button"
									value="S"
								/>
							</form>
							<div class="success-message w-form-done">
								<div class="text-success">Thank you! Your submission has been received!</div>
							</div>
							<div class="w-form-fail">
								<div>Oops! Something went wrong while submitting the form.</div>
							</div>
						</div>
					</div>
				</div> -->
				<div class="flex-elements margin-top-40">
					<div class="copyright">
						<div>© IRLY APP - All Right Reserved 2022</div>
					</div>
					<div class="social-icons">
						<a href="#" class="social-link w-inline-block">
							<img src="images/63486f026e1d1728ffd7d238_icon-fb.svg" loading="lazy" alt="" />
						</a>
						<a href="#" class="social-link w-inline-block">
							<img src="images/63486f026e1d17ecbdd7d239_icon-twitter.svg" loading="lazy" alt="" />
						</a>
						<a href="#" class="social-link w-inline-block">
							<img src="images/63486f026e1d176cd4d7d23a_icon-youtube.svg" loading="lazy" alt="" />
						</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>

<Hero />

<Features />

<Gallery />

<Faq />

<!-- <Cta /> -->

<Footer />

<style lang="postcss">
</style>
