<script lang="ts">
	import Header from '../lib/components/ui/Layout/Header.svelte';
	import Intro from '../lib/components/ui/Layout/Intro.svelte';
	import Main from '../lib/components/ui/Layout/Main.svelte';
	import '../app.pcss';
</script>

<Header/>
<Intro/>
<Main/>
<slot />
