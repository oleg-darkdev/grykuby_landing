<script lang="ts">
	// import {  } from '$shared';
	// import {  } from '$widgets';
	// import {  } from '$entities'
</script>

<div class="promo-card _1">
	<div class="content-promo-card">
		<div class="title-promo-card">Lorem impsum</div>
	</div>
</div>

<div class="promo-card _2">
	<div class="content-promo-card">
		<div class="title-promo-card">Lorem impsum</div>
	</div>
</div>

<style lang="postcss">
	.number-promo-card {
		color: var(--blue-violet);
		text-shadow:
			-1px 0 0 var(--white),
			0 1px 0 var(--white),
			1px 0 0 var(--white),
			0 -1px 0 #fff;
		cursor: default;
		font-family: Termina, sans-serif;
		font-size: 32px;
		font-weight: 900;
		line-height: 38px;
		position: absolute;
		inset: auto 0% 0% auto;
	}

	.promo-card {
		border: 6px solid #fff;
		border-radius: 36px;
		flex-direction: column;
		justify-content: space-between;
		width: 332px;
		height: 495px;
		padding: 24px;
		display: flex;
		position: relative;
	}

	.promo-card._1 {
		z-index: 5;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%),
			url('/images/avatar-card-3-min.webp');
		/*  */
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
	}

	.promo-card._2 {
		z-index: 5;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%),
			url('/images/avatar-card-3-min.webp');
		/* 63486f026e1d178d70d7d231_img-promo-card-2-min.webp*/
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		position: absolute;
		top: 105px;
		left: 234px;
	}

	.promo-card._3 {
		z-index: 4;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%), url('');
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		position: absolute;
		inset: 0% auto auto 0%;
	}

	.promo-card._4 {
		z-index: 3;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%), url('');
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		position: absolute;
		inset: 0% auto auto 0%;
	}

	.promo-card._5 {
		z-index: 2;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%), url('');
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		position: absolute;
		inset: 0% auto auto 0%;
	}

	.promo-card._6 {
		z-index: 1;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%), url('');
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		position: absolute;
		inset: 0% auto auto 0%;
	}

	.promo-card._7 {
		z-index: 0;
		background-image: linear-gradient(#765bfa00 50%, #6041f7 89%), url('');
		background-position:
			0 0,
			50%;
		background-size: auto, cover;
		display: none;
		position: absolute;
		inset: 0% auto auto 0%;
	}

	.content-promo-card {
		position: relative;
	}

	.title-promo-card {
		cursor: default;
		font-family: Termina, sans-serif;
		font-size: 32px;
		font-weight: 700;
		line-height: 38px;
	}

	@media screen and (max-width: 991px) {
		.title-promo-card {
			font-size: 24px;
			line-height: 30px;
		}
	}

	@media screen and (max-width: 479px) {
		.promo-card {
			width: 100%;
			height: 400px;
		}

		.promo-card._2,
		.promo-card._3,
		.promo-card._4,
		.promo-card._5,
		.promo-card._6 {
			position: static;
		}
		.number-promo-card {
			font-size: 24px;
			line-height: 24px;
			bottom: 5px;
		}
	}
</style>
