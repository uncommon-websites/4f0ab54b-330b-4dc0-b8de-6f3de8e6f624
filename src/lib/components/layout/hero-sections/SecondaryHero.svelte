<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="border-b border-gray-100 dark:border-gray-900 bg-gradient-to-br from-white to-gray-50" {...rest}>
	<div class="section-px section-py container mx-auto grid gap-16 gap-y-0">
		<div class="container-sm grid text-balance text-center space-y-4">
			<h1 class="text-display font-medium">
				<span class="text-primary-600">{title}</span>
			</h1>
			<p class="text-title2 text-emphasis-medium max-w-2xl mx-auto leading-relaxed">
				{subtitle}
			</p>
		</div>
		<div class="aspect-video overflow-clip rounded-xl bg-gradient-to-br from-primary-50 to-primary-100 border border-primary-200 relative">
			<img
				class="h-full w-full object-cover rounded-xl hover:scale-105 transition-transform duration-700"
				src={imageSrc}
				alt="Team collaborating on presentation design in modern workspace"
			/>
			<div class="absolute inset-0 bg-gradient-to-t from-primary-600/10 to-transparent pointer-events-none rounded-xl"></div>
		</div>
	</div>
</header>
