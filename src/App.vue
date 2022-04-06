<script setup>
import AppHeader from './components/AppHeader.vue';
import AppGrid from './components/AppGrid.vue';
import AppBadge from './components/AppBadge.vue';
import AppSidebar from './components/AppSidebar.vue';
</script>

<template>
	<div class="page__content">
		<AppHeader />

		<div class="main__content">
			<AppSidebar />
			<div>
				<div class="badge__container">
					<AppBadge v-for="i in 20">Comedies {{ i }}</AppBadge>
				</div>

				<AppGrid />

				<footer class="p-3 bg-yellow-100 text-center sticky bottom-0">
					Made with ❤️ by Students
				</footer>
			</div>
		</div>
	</div>
</template>

<style scoped>
.main__content {
	display: grid;
	grid-template-columns: auto minmax(0, 1fr);
}

.page__content {
	display: grid;
	grid-template-rows: auto minmax(0, 1fr);
}

.badge__container {
	display: flex;
	gap: 14px;
	padding: 0.5rem 1rem;
	position: sticky;
	top: 62px;
	z-index: 1;
	background-color: rgba(255, 255, 255, 0.9);
	overflow-x: auto;
	border-top: 1px solid gray;
	border-bottom: 1px solid gray;
}
</style>
