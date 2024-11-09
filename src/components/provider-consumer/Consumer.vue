<template>
	<div>Injected User: {{ user }}</div>
</template>

<script>
	export default {
		inject: ["user"],
	};
</script>
