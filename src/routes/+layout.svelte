<script lang="ts">
	import './layout.css';
	import '@patternfly/patternfly/patternfly.css';
	import '@patternfly/patternfly/patternfly-addons.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
{@render children()}
