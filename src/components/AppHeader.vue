<script setup>
import AppLogo from './AppLogo.vue';
import SearchIcon from '../icons/SearchIcon.vue';
</script>

<template>
	<header>
		<AppLogo class="w-24" />
		<form>
			<input type="text" />
			<button>
				<SearchIcon />
			</button>
		</form>
		<img src="https://picsum.photos/100/100" class="w-8 h-8 rounded-full" />
	</header>
</template>

<style scoped>
header {
	position: sticky;
	top: 0px;
	z-index: 1;
	background-color: rgba(255, 255, 255, 0.9);
	padding: 1rem;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

form {
	display: flex;
	border: 1px solid #ccc;
}

button {
	background-color: #f0f0f0;
	padding: 10px;
	height: 100%;
}
</style>
