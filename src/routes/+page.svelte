<script lang="ts">
	import profileImage from '$lib/assets/profile_image.webp';
	import profileImageMobile from '$lib/assets/profile_image_m.webp';
	import profileImageFallback from '$lib/assets/profile_image.jpg';
</script>

<svelte:head>
	<title>Okunola Joshua | Portfolio</title>
	<meta
		name="description"
		content="Okunola Joshua's Personal site. I am a frontend, Javascript and Typescript developer.Vast experience with  react, svelte, next js."
	/>
</svelte:head>

<main class="min-h-screen  grid place-content-center antialiased ">
	<div
		class="container mx-auto md:grid grid-cols-[1fr_2fr] place-content-center items-stretch justify-center"
	>
		<div class="px-6 pt-6 flex items-center ">
			<picture class="object-fill mx-auto">
				<source media="(max-width:640px)" srcset={profileImageMobile} width="640" height="640" />
				<source media="(min-width: 641px)" srcset={profileImage} width="640" />
				<img
					width="400"
					class="grayscale rounded-3xl mx-auto w-screen lg:w-full"
					src={profileImageFallback}
					alt="Okunola's profile"
				/>
			</picture>
		</div>
		<div class=" flex p-6">
			<div class="flex flex-col gap-6 justify-between">
				<header>
					<h1 class="text-3xl lg:text-6xl xl:text-8xl font-bold">Hi, I'm Okunola Joshua.</h1>
				</header>
				<section>
					<p class="text-base  lg:text-2xl">
						I'm a 27 years old Javascript / frontend developer who cares about the various
						technology that are related to the web. I have experience with react js and svelte.
					</p>
				</section>

				<section class="">
					<h2 class="font-semibold text-xl lg:text-2xl mb-4"><span>Contact</span></h2>
					<ul class="flex flex-col gap-2 text-base lg:text-xl">
						<li><a href="tel:+7(927)043-47-22">+7(927)043-47-22</a></li>
						<li class="underline">
							<span /><a target="_blank" href="mailto:a.joshua.okunola@gmail.com"
								><span>a.joshua.okunola@gmail.com</span></a
							><span />
						</li>
						<li><a href="https://github.com/AfoeJoe">Github</a></li>
						<li><a href="https://www.linkedin.com/in/okunola-joshua/">LinkedIn</a></li>
					</ul>
				</section>
			</div>
		</div>
	</div>
</main>

<style lang="postcss">
	:global(p) {
		font-size: theme(fontSize.xl);
		line-height: 1.5;
	}
</style>
