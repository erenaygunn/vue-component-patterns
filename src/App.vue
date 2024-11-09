<script setup>
	import Container from "./components/container/Container.vue";
	import Dynamic from "./components/dynamic-components/Dynamic.vue";
	import Mixin from "./components/mixins/Mixin.vue";
	import Parent from "./components/provide-inject/Parent.vue";
	import Provider from "./components/provider-consumer/Provider.vue";
	import Adapter from "./components/Adapter.vue";
	import FormBuilder from "./components/FormBuilder.vue";
	import Functional from "./components/Functional.vue";
	import Renderless from "./components/Renderless.vue";
	import SFC from "./components/SFC.vue";
	import Slots from "./components/Slots.vue";
	import Teleport from "./components/Teleport.vue";
	import TemplateLiteral from "./components/TemplateLiteral.vue";
</script>

<template>
	<div>
		<h1>Vue Component Patterns Showcase</h1>

		<section>
			<h2>Container/Presentational</h2>
			<Container />
		</section>

		<section>
			<h2>Dynamic Components</h2>
			<Dynamic />
		</section>

		<section>
			<h2>Mixins</h2>
			<Mixin />
		</section>

		<section>
			<h2>Provide-Inject</h2>
			<Parent />
		</section>

		<section>
			<h2>Provider-Consumer</h2>
			<Provider>
				<Consumer />
			</Provider>
		</section>

		<section>
			<h2>Adapter</h2>
			<Adapter />
		</section>

		<section>
			<h2>FormBuilder</h2>
			<FormBuilder>
				<template v-slot="{ formData, updateField }">
					<div>
						<label>Name:</label>
						<input
							type="text"
							v-model="formData.name"
							@input="updateField('name', $event.target.value)"
						/>
					</div>
					<div>
						<label>Age:</label>
						<input
							type="number"
							v-model="formData.age"
							@input="updateField('age', $event.target.value)"
						/>
					</div>
				</template>
			</FormBuilder>
		</section>

		<section>
			<h2>Functional</h2>
			<Functional message="Hello from functional component!" />
		</section>

		<section>
			<h2>Renderless</h2>
			<Renderless url="https://jsonplaceholder.typicode.com/posts/1" />
		</section>

		<section>
			<h2>SFC</h2>
			<SFC />
		</section>

		<section>
			<h2>Slots</h2>
			<Slots>
				<template #header>Custom Header</template>
				<template>Custom Body Content</template>
				<template #footer>Custom Footer</template>
			</Slots>
		</section>

		<section>
			<h2>Teleport</h2>
			<Teleport />
		</section>

		<section>
			<h2>Template Literal</h2>
			<TemplateLiteral />
		</section>
	</div>
</template>

<style scoped>
	h1 {
		text-align: center;
		margin-bottom: 20px;
	}
	section {
		margin-bottom: 40px;
	}
</style>
