<script>
	import { browser } from '$app/environment';
	import '../app.postcss';

	if (browser) document.documentElement.classList.add('dark');
</script>

<div class="m-5">
	<slot />
</div>
