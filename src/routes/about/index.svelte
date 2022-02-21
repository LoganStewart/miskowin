<script lang="ts">
	// Start: Local Imports
	// Components
	import HeadTags from '$components/head-tags/HeadTags.svelte';
	import ExternalLink from '$ui/components/external-link/ExternalLink.svelte';

	// Models
	import type { IMetaTagProperties } from '$models/interfaces/imeta-tag-properties.interface';
	// End: Local Imports

	// Start: Local component properties
	/**
	 * @type {IMetaTagProperties}
	 */
	const metaData: Partial<IMetaTagProperties> = {
		title: 'About | Sveltekit Blog',
		description: 'About page of Sveltekit blog starter project',
		url: '/about',
		keywords: ['sveltekit', 'sveltekit starter', 'sveltekit starter about'],
		searchUrl: '/about',
	};
	// End: Local component properties
</script>

<!-- Start: Header Tag -->
<HeadTags metaData="{metaData}" />
<!-- End: Header Tag -->

<!-- Start: About page section -->
<div class="flex flex-col justify-center items-start max-w-2xl mx-auto mb-16">
	<h1 class="font-bold text-3xl md:text-5xl tracking-tight mb-4 text-black dark:text-white"> About Me </h1>
	<div class="mb-8 prose leading-6 text-gray-600 dark:text-gray-400">
		<p>
			Hey, I'm Logan, a full-stack developer,  well I am a little more than that. I have a passion for CI/CD and the process of software development.  
			I really enjoy working with people and I am always looking to learn new things. 

		</p>
		<p>
		I have recently been working with the Power Platform and I am very excited to see what the future holds for it.  
			Although there are so so many things that need to be improved with the professional developer/operations experience, I think it is off to a good start.
		</p>
		<p>
			I am quite interested in Svelte to see where it goes (I have developed this blog and site with it.)
		</p>
		<p>
			I will post contact details here as well as my GitHub and other social media links.
		</p>
	
	</div>
</div>
<!-- End: About page section -->
