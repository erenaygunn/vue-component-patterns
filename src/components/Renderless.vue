<template v-if="false"></template>

<script>
	export default {
		props: ["url"],
		data() {
			return { data: null };
		},
		mounted() {
			fetch(this.url)
				.then((res) => res.json())
				.then((data) => (this.data = data));
		},
	};
</script>
