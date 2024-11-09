<template>
	<PresentationalComponent :message="message" />
</template>

<script>
	import PresentationalComponent from "./Presentational.vue";
	export default {
		components: { PresentationalComponent },
		data() {
			return { message: "Hello from the container!" };
		},
	};
</script>
