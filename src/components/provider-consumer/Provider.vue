<template>
	<div>
		<p>This is the provider component.</p>
		<slot></slot>
	</div>
</template>

<script>
	export default {
		data() {
			return { user: "User123" };
		},
		provide() {
			return { user: this.user };
		},
	};
</script>
