<template>
	<div id="app" class="m-20">
		<img alt="Vue logo" class="mb-20" src="./assets/logo.png" />
		<div
			class="grid w-40 bg-green-600 rounded hover:bg-white duration-200 delay-300"
			@mouseenter="trigger = false"
			@mouseleave="trigger = true"
		>
			<div class=""></div>
			<Motion
				v-model="trigger"
				:trigger="['rounded', 'rounded-t', 'rounded']"
				class="z-10 origin-top-left bg-green-600 h-12"
			/>
			<Motion
				v-model="trigger"
				:trigger="[
					'rounded-none -translate-y-12 opacity-0 scale-75 h-0',
					'translate-y-0 opacity-100 scale-100 h-12',
					'mt-1 rounded',
				]"
				class="bg-green-600 hover:bg-green-700 cursor-pointer"
			/>

			<Motion
				v-model="trigger"
				:trigger="[
					'rounded-none -translate-y-12 opacity-0 scale-75 h-0',
					'translate-y-0 opacity-100 scale-100 h-12',
					'mt-1 rounded',
				]"
				class="bg-green-600 hover:bg-green-700 cursor-pointer"
			/>
			<Motion
				v-model="trigger"
				:trigger="[
					'rounded-none -translate-y-12 opacity-0 scale-75 h-0',
					'translate-y-0 opacity-100 scale-100 h-12',
					'mt-1 rounded',
				]"
				class="bg-green-600 hover:bg-green-700 cursor-pointer"
			/>
			<Motion
				v-model="trigger"
				:trigger="[
					'rounded-none -translate-y-12 opacity-0 scale-75 h-0',
					'translate-y-0 opacity-100 scale-100 h-12 rounded-b',
					'mt-1 rounded',
				]"
				class="bg-green-600 hover:bg-green-700 cursor-pointer"
			/>
		</div>
		<div>test</div>
	</div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Motion from "tinymotion";

export default {
	name: "App",
	components: {
		// HelloWorld,
		Motion,
	},
	data() {
		return {
			trigger: true,
		};
	},
};
</script>

<style>
/* #app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
} */
</style>
