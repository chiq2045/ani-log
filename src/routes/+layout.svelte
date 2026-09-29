<script lang="ts">
	import './layout.css';
	import '@patternfly/patternfly/patternfly.css';
	import '@patternfly/patternfly/patternfly-addons.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="pf-v6-c-page">
	<header class="pf-v6-c-masthead">
		<div class="pf-v6-c-masthead__main">
			<span class="pf-v6-c-masthead__toggle">
				<button
					class="pf-v6-c-button pf-m-hamburger pf-m-plain"
					type="button"
					aria-label="Global navigation"
				>
					<span class="pf-v6-c-button__icon">
						<svg
							viewBox="0 0 10 10"
							class="pf-v6-c-button--hamburger-icon pf-v6-svg"
							width="1em"
							height="1em"
						>
							<path class="pf-v6-c-button--hamburger-icon--top" d="M1,1 L9,1" />
							<path class="pf-v6-c-button--hamburger-icon--middle" d="M1,5 L9,5" />
							<path class="pf-v6-c-button--hamburger-icon--arrow" d="M1,5 L1,5 L1,5" />
							<path class="pf-v6-c-button--hamburger-icon--bottom" d="M9,9 L1,9" />
						</svg>
					</span>
				</button>
			</span>
			<div class="pf-v6-c-masthead__brand">
				<a class="pf-v6-c-masthead__logo" href="#">Logo</a>
			</div>
		</div>
		<div class="pf-v6-c-masthead__content">
			<span>Content</span>
		</div>
	</header>
	<div class="pf-v6-c-page__main-container pf-m-fill" tabindex="-1">
		<main class="pf-v6-c-page__main" tabindex="-1">
			{@render children()}
			<!-- <section class="pf-v6-c-page__main-section" aria-label="Regular page section example"> -->
			<!-- 	<div class="pf-v6-c-page__main-body">A regular page section.</div> -->
			<!-- </section> -->
			<!-- <section class="pf-v6-c-page__main-section pf-m-fill" aria-label="Fill page section example"> -->
			<!-- 	<div class="pf-v6-c-page__main-body"> -->
			<!-- 		This section uses -->
			<!-- 		<code>.pf-m-fill</code> to fill the available space. The -->
			<!-- 		<code>.pf-v6-c-page__main-container</code> must also have -->
			<!-- 		<code>.pf-m-fill</code> in order for the section to have space to stretch to full height. -->
			<!-- 	</div> -->
			<!-- </section> -->
			<!-- <section -->
			<!-- 	class="pf-v6-c-page__main-section pf-m-no-fill" -->
			<!-- 	aria-label="No fill page section example" -->
			<!-- > -->
			<!-- 	<div class="pf-v6-c-page__main-body"> -->
			<!-- 		This section uses -->
			<!-- 		<code>.pf-m-no-fill</code> and will not fill the available space. -->
			<!-- 	</div> -->
			<!-- </section> -->
		</main>
	</div>
</div>
