<script>
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
<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/flickity@2/dist/flickity.min.css" />
	<script src="https://unpkg.com/flickity@2/dist/flickity.pkgd.min.js"></script>
</svelte:head>

<div class="main-carousel">
	<div class="carousel-cell">...</div>
	<div class="carousel-cell">...</div>
	<div class="carousel-cell">...</div>
</div>

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
