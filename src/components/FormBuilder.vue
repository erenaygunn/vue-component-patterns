<template>
	<form @submit.prevent="submitForm">
		<slot
			:formData="formData"
			:updateField="updateField"
		></slot>
		<button type="submit">Submit</button>
	</form>
</template>

<script>
	export default {
		data() {
			return { formData: { name: "", age: "" } };
		},
		methods: {
			updateField(field, value) {
				this.formData[field] = value;
			},
			submitForm() {
				console.log("Form submitted:", this.formData);
			},
		},
	};
</script>
