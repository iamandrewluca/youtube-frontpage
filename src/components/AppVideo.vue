<script setup>
defineProps({
	image: String,
	avatar: String,
});
</script>

<template>
	<div>
		<div class="relative">
			<img :src="image" class="aspect-video object-cover" />
			<span class="video__time">14:10</span>
		</div>

		<div class="flex gap-3 items-start mt-2">
			<img :src="avatar" class="rounded-full" />
			<div class="grow">
				<h4 class="line-clamp-2 video__title">
					<span class="video__subtitle">Playing Fortnite</span>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam,
					consectetur?
				</h4>

				<div class="text-sm text-gray-500">
					<div>extratv</div>
					<div>12M views . 2 days ago</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.video__subtitle {
	font-size: 1.2rem;
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
</style>
