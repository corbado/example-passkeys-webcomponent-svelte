<script lang="ts">
	import Footer from '$lib/sections/Footer.svelte';
	import PasskeyDemo from '$lib/sections/PasskeyDemo.svelte';
	import PasskeyExplainer from '$lib/sections/PasskeyExplainer.svelte';
	import PasskeySaas from '$lib/sections/PasskeySaas.svelte';
	import PasskeyStats from '$lib/sections/PasskeyStats.svelte';
	import PasskeyTimeline from '$lib/sections/PasskeyTimeline.svelte';
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.bunny.net" />
	<link rel="preconnect" href="https://fonts.bunny.net" />
	<link
		href="https://fonts.bunny.net/css?family=inter:100,200,300,400,500,600,700,800,900|space-grotesk:300,400,500,600,700"
		rel="stylesheet"
	/>
	<title>Passkeys demo</title>
	<meta name="description" content="Corbado Passkey passwordless authentication demo" />
	<meta property="og:title" content="Corbado Passkeys demo" />
	<meta
		property="og:description"
		content="Corbado Passkey passwordless authentication demo using passkeys"
	/>
	<meta property="og:image" content="share_image.png" />
	<meta property="og:url" content="https://passkeys.eu" />
	<meta property="og:type" content="website" />
</svelte:head>

<PasskeyDemo {data} />

<PasskeyExplainer />

<PasskeyTimeline />

<PasskeyStats />

<PasskeySaas />

<Footer />
