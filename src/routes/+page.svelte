<script lang="ts">
	let count = $state(0)
</script>

<h1>Welcome to SvelteKit</h1>
<p>Counter example:</p>
<button onclick={() => count++}>
	clicks: {count}
</button>
