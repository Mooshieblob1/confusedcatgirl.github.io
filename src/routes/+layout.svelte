<script>
	import '../app.css';

	const links = [
		{ href: '/', label: 'Home' },
		{ href: '/#cloud', label: 'Cloud' },
		{ href: '/#projects', label: '3D-Printed Projects' },
		{ href: '/#contact', label: 'Contact' },
		{ href: '/tos', label: 'Terms of Service' }
	];
</script>

<svelte:head>
	<title>Blorb's Website</title>
	<link rel="icon" href="https://confusedblorb.org/icon.png" />
</svelte:head>

<!-- Full viewport and background -->
<div
	class="flex min-h-screen flex-col bg-cover bg-fixed bg-center text-white"
	style="background-image: url('https://raw.githubusercontent.com/confusedcatgirl/confusedcatgirl.github.io/refs/heads/main/background.webp');"
>
	<img src="https://confusedblorb.org/blorb.webp" alt="Banner" class="mx-auto w-[38%] pt-4" />

	<nav
		class="m-4 flex flex-wrap justify-center gap-4 rounded-lg bg-indigo-900/40 p-2 backdrop-blur"
	>
		{#each links as { href, label }}
			<a
				{href}
				class="rounded-lg bg-gradient-to-b from-indigo-200 to-indigo-400 px-4 py-2 text-sm font-medium text-black hover:from-indigo-400 hover:to-indigo-200"
			>
				{label}
			</a>
		{/each}
	</nav>

	<!-- Slot grows to fill, prevents collapsing on short pages -->
	<main class="flex-1">
		<slot />
	</main>

	<!-- Footer About section -->
	<footer class="text_area mt-16">
		<h2 class="mb-2 text-2xl font-bold">About</h2>
		<p>© 2023 - 2025 confusedcatgirl</p>
		<p class="pl-8">
			Banner by <a href="https://www.mooshieblob.com/" class="underline">mooshieblob 2024</a>
		</p>
		<p class="pl-8">
			Image by <a href="https://danbooru.donmai.us/posts/1029426" class="underline"
				>Yuuki Tatsuya 2011</a
			>
		</p>
	</footer>
</div>
