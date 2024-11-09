<template>
	<div v-html="templateContent"></div>
</template>

<script>
	export default {
		data() {
			return {
				templateContent: "<p>This is a template literal example.</p>",
			};
		},
	};
</script>
