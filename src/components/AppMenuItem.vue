<script setup>
import GridIcon from '../icons/GridIcon.vue';

defineProps({
	title: String,
});
</script>

<template>
	<button class="menu__item">
		<slot name="icon">
			<GridIcon class="w-6 h-6" />
		</slot>
		<span class="hidden sm:block">{{ title }}</span>
	</button>
</template>

<style scoped>
.menu__item {
	width: 100%;
	display: flex;
	gap: 1rem;
	padding: 0.5rem;
	align-items: center;
}

.menu__item:hover {
	background-color: #eee;
}

.menu__item:focus {
	background-color: yellow;
}
</style>
