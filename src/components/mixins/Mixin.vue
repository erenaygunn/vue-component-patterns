<template></template>

<script>
	import myMixin from "./myMixin.js";
	export default {
		mixins: [myMixin],
		template: `<p>{{ mixinData }}</p>`,
	};
</script>
