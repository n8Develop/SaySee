<script>
	import { register } from 'swiper/element/bundle';

	register();

	const spaceBetween = 10;

	const onProgress = (e) => {
		const [swiper, progress] = e.detail;
		console.log(progress);
	};

	const onSlideChange = (e) => {
		console.log('slide changed');
	};
</script>

<!-- <div class="container">
  <div class="left">
    <div class="leftItems">Left Arrow</div>
  </div>

  <div class="middle">
    <div class="middleItems">Carousel Placeholder</div>
  </div>

  <div class="right">
    <div class="rightItems">Right Arrow</div>
  </div>
</div> -->
<swiper-container
	slides-per-view={3}
	space-between={spaceBetween}
	centered-slides={true}
	pagination={{
		hideOnClick: true
	}}
	breakpoints={{
		768: {
			slidesPerView: 3
		}
	}}
	on:progress={onProgress}
	on:slidechange={onSlideChange}
>
	<swiper-slide>Slide 1</swiper-slide>
	<swiper-slide>Slide 2</swiper-slide>
	<swiper-slide>Slide 3</swiper-slide>
</swiper-container>

<style>
	.gallery-cell {
		width: 66%;
		height: 100px;
		margin-right: 10px;
		background: #fff68f;
	}

	.container {
		grid-template-columns: 20%[left] 60% [middle] 20% [right];
		grid-template-areas: 'left middle right';
		display: grid;
	}

	.left {
		background-color: rgb(197, 63, 161, 0.4);
		grid-column-start: left;
	}
	.leftItems {
		justify-self: center;
	}
	.middle {
		background-color: rgb(17, 163, 161, 0.4);
		grid-column-start: middle;
	}
	.middleItems {
		justify-self: center;
	}
	.right {
		background-color: rgb(97, 63, 61, 0.4);
		grid-column-start: right;
	}
	.rightItems {
		justify-self: center;
	}
</style>
