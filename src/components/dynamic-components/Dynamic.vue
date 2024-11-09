<template>
	<component :is="currentComponent"></component>
	<button @click="toggleComponent">Switch</button>
</template>

<script>
	import ComponentA from "./ComponentA.vue";
	import ComponentB from "./ComponentB.vue";

	export default {
		data() {
			return { currentComponent: "ComponentA" };
		},
		components: { ComponentA, ComponentB },
		methods: {
			toggleComponent() {
				this.currentComponent =
					this.currentComponent === "ComponentA" ? "ComponentB" : "ComponentA";
			},
		},
	};
</script>
