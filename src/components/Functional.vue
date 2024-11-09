<template>
	<div>I'm a functional component. My prop is: {{ $props.message }}</div>
</template>

<script>
	export default {
		props: {
			message: String,
		},
	};
</script>
