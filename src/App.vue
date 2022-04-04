<script setup>
import AppHeader from './components/AppHeader.vue';
import AppGrid from './components/AppGrid.vue';
import AppBadge from './components/AppBadge.vue';
</script>

<template>
	<AppHeader />
	<div>
		<div class="badge__container">
			<AppBadge v-for="i in 20">Comedies {{ i }}</AppBadge>
		</div>

		<AppGrid />
	</div>
</template>

<style scoped>
.badge__container {
	display: flex;
	gap: 14px;
	padding: 0.5rem 1rem;
	position: sticky;
	top: 78px;
	z-index: 1;
	background-color: rgba(255, 255, 255, 0.9);
	overflow-x: auto;
}
</style>
