<script lang="ts">
	// import {  } from '$widgetsLanding';
	// import { } from '$sharedData';
	import '../../../app/app.css';

	let { children } = $props();
</script>

<!-- overflow-hidden -->
<div class="body ">
	{@render children()	}
</div>

<style lang="postcss">
</style>
