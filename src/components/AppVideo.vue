<template>
	<div>
		<div class="video__wrapper">
			<img src="https://picsum.photos/1080/1920" class="video__image" />
			<span class="video__time">14:10</span>
		</div>

		<h4 class="video__title">Playing Fortnite all day</h4>
	</div>
</template>

<style>
.video__image {
	display: block;
	max-width: 100%;
	aspect-ratio: 2 / 1;
	object-fit: cover;
}

.video__title {
	margin-top: 0px;
	margin-bottom: 0px;
}

.video__time {
	background-color: black;
	color: white;
	padding: 5px;
	font-size: 14px;
	position: absolute;
	bottom: 0px;
	right: 0px;
}

.video__wrapper {
	display: inline-block;
	position: relative;
}
</style>
