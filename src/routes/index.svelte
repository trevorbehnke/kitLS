<!-- App.svelte -->
<script>
	import Todos from '$lib/components/Todos.svelte';
	import Alert from '$lib/components/Alert.svelte';
	import { todos } from '../stores.js';
</script>

<Alert />
<Todos bind:todos={$todos} />

<!-- <script context="module">
	export const ssr = false;
	import { todos } from '../stores/stores';
</script>

<main>
	{#each $todos as { id, name, completed }}
		<section>
			{id}: {name} - {completed}
		</section>
	{/each}
</main> -->
