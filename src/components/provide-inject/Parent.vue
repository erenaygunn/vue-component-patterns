<template><Child /></template>

<script>
	import Child from "./Child.vue";
	export default {
		components: { Child },
		provide: { message: "Hello from parent" },
	};
</script>
