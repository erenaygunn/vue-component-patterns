<template><button @click="handleClick">Click me</button></template>

<script>
	export default {
		methods: {
			handleClick() {
				ThirdPartyLib.doSomething();
			},
		},
	};
</script>
