<script setup>
import AppVideo from './components/AppVideo.vue';
</script>

<template>
	<div class="app__grid">
		<AppVideo v-for="i in 10" />
	</div>
</template>

<style>
.app__grid {
	display: grid;
	grid-template-columns: repeat(4, 1fr);
	gap: 20px;
}
</style>
