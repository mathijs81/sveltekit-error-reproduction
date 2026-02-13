<script lang="ts">
  import { error } from "@sveltejs/kit";
</script>

<a href="/">Home</a> | <a href="/route1">Route 1</a> | <a href="/route2">Route 2</a> <br/>

<strong>Bad routes:</strong><br/>

<button on:click={() => {
	throw new Error('Test error');
}}>Throw error</button>

<button on:click={() => {
	throw error(500, "My custom error message");
}}>throw svelte error</button>

<a href="/bad-route-regular">Route that throws Error</a> | <a href="/bad-route-svelte">Route that throws Svelte error</a> | <a href="/non-existent-route">Non-existent route</a>