<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)

const increaseCount = () => {
	count.value += 1
}
</script>

<template>
	<h1>{{ msg }}</h1>

	<div class="card">
		<button type="button" @click.prevent="increaseCount">count is {{ count }}</button>
		<div
			wow="1"
			zz="1"
			veryLongAttribute="this is very long attribute."
			veryLongAttributeTwo="this is very long attribute."
		/>
		<p>
			Edit
			<code>components/HelloWorld.vue</code> to test HMR
		</p>
	</div>

	<p>
		Check out
		<a href="https://vuejs.org/guide/quick-start.html#local" target="_blank">create-vue</a>, the official Vue + Vite
		starter
	</p>
	<p>
		Install
		<a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
		in your IDE for a better DX
	</p>
	<p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
	color: #888;
}
</style>
