<script>
	const socialSafe = [
		{
			href: 'https://twitch.tv/confusedcatgirl',
			icon: 'https://confusedblorb.org/icons/twitch.webp'
		},
		{
			href: 'https://github.com/confusedcatgirl',
			icon: 'https://confusedblorb.org/icons/github.webp'
		}
	];

	const socialNSFW = [
		{ href: 'https://x.com/darkmothlady', icon: 'https://confusedblorb.org/icons/twitter.webp' },
		{
			href: 'https://anilist.co/user/confusedcatgirl',
			icon: 'https://confusedblorb.org/icons/anilist.webp'
		},
		{
			href: 'https://www.deviantart.com/confusedcatgirl',
			icon: 'https://confusedblorb.org/icons/deviantart.webp'
		}
	];

	const projects = Array.from(
		{ length: 8 },
		(_, i) => `https://confusedblorb.org/projects/${i + 1}.jpg`
	);
</script>

<section id="home" class="text_area">
	<h2 class="mb-2 text-2xl font-bold">Home</h2>
	<p class="mb-1">Welcome to my little page!</p>
	<p>I am Blorb, also known as confusedcatgirl, and I generated AI Artifacts as a Hobby!</p>
	<p>I like to draw sometimes, and code in various languages from time to time.</p>
	<p>Most of the time, I am pretty laid back, and I like to talk about video games too!</p>
	<p>I like to mess around with game engines, and see what I can make with them.</p>
	<p>I am a former user of AI, due to various reasons, including my own mental health.</p>
	<p>Now, I 3d print models and paint them as a hobby, I might even share them on here!</p>
	<p>This page is rather short as of right now, but I hope to extend it into a lot more!</p>
</section>

<section id="cloud" class="text_area">
	<h2 class="mb-2 text-2xl font-bold">Cloud</h2>
	<p>This server is only available to a select few. It uses HSTS + HTTPS.</p>
	<p>Based on Nextcloud — check the original software out!</p>
	<a href="https://cloud.confusedblorb.org/index.php/" class="button"
		>Continue to the Cloud Login (disabled)</a
	>
</section>

<section id="projects" class="text_area">
	<h2 class="mb-4 text-2xl font-bold">3D-Printed Projects</h2>
	<div class="flex flex-wrap justify-center gap-4">
		{#each projects as url}
			<img src={url} alt="3D Project" class="h-[200px] w-1/3 rounded-lg object-cover" />
		{/each}
	</div>
</section>

<section id="contact" class="text_area">
	<h2 class="mb-2 text-2xl font-bold">Contact</h2>

	<p class="text-center">Safe for Work:</p>
	<div class="my-2 flex justify-center gap-4">
		{#each socialSafe as { href, icon }}
			<a {href}><img src={icon} alt="icon" class="w-12 invert" /></a>
		{/each}
	</div>

	<p class="text-center">Contains NSFW:</p>
	<div class="my-2 flex justify-center gap-4">
		{#each socialNSFW as { href, icon }}
			<a {href}><img src={icon} alt="icon" class="w-12 invert" /></a>
		{/each}
	</div>
</section>

<section id="tos" class="text_area">
	<h2 class="mb-2 text-2xl font-bold">Terms of Service</h2>
	<p>Using this website automatically counts as an agreement to Terms of Service.</p>
	<a href="/tos" class="button">Continue to TOS</a>
</section>
