<script>
	import { ModeWatcher } from "mode-watcher"
	import { Toaster } from "$lib/components/ui/sonner";

	import Header from "$lib/components/header.svelte";
	import Footer from "$lib/components/footer.svelte";

	import '../app.css'
	import 'iconify-icon'
</script>

<ModeWatcher />
<Toaster />
<div class="max-w-6xl mx-auto min-h-screen layout">
	<Header />
	<main>
		<slot />
	</main>
	<Footer />
</div>

<style>
	.layout {
		display: grid;
		grid-template-rows: auto 1fr auto;
	}
</style>
