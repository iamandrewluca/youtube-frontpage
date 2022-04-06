<script setup>
import AppMenuItem from './AppMenuItem.vue';
import VideoIcon from '../icons/VideoIcon.vue';
import BellIcon from '../icons/BellIcon.vue';
</script>

<template>
	<aside>
		<div class="menu__block">
			<AppMenuItem title="Home">
				<template #icon>
					<BellIcon class="w-6 h-6" />
				</template>
			</AppMenuItem>

			<AppMenuItem title="Explore">
				<template #icon>
					<VideoIcon class="w-6 h-6" />
				</template>
			</AppMenuItem>
		</div>

		<div class="menu__block">
			<h3>Subscriptions</h3>
			<AppMenuItem title="Library" />
			<AppMenuItem title="History" />
			<AppMenuItem title="Your Videos" />
			<AppMenuItem title="Watch Later" />
		</div>

		<div class="menu__block">
			<h3>More from YouTube</h3>
			<AppMenuItem title="Liked Videos" />
			<AppMenuItem title="Gaming" />
			<AppMenuItem title="Live" />
			<AppMenuItem title="Learning" />
		</div>
	</aside>
</template>

<style scoped>
.menu__block {
	padding: 1rem;
}

.menu__block + .menu__block {
	border-top: 1px solid gray;
}

.menu__block > h3 {
	display: none;
}

@media (min-width: 640px) {
	.menu__block > h3 {
		display: block;
		font-weight: 700;
		color: gray;
		text-transform: uppercase;
		font-size: 0.9rem;
		margin-bottom: 0.5rem;
	}
}
</style>
