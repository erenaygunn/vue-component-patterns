<template>
	<div class="card">
		<div class="card-header">
			<slot name="header">Default Header</slot>
		</div>
		<div class="card-body">
			<slot>Default Body Content</slot>
		</div>
		<div class="card-footer">
			<slot name="footer">Default Footer</slot>
		</div>
	</div>
</template>

<style>
	.card {
		border: 1px solid #ddd;
		padding: 10px;
	}
	.card-header,
	.card-footer {
		font-weight: bold;
	}
</style>
