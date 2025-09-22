<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Design thinking",
			description: "Every feature starts with design principles. We build AI that thinks like designers, creating beautiful presentations that preserve your brand identity."
		},
		{
			title: "Speed without sacrifice",
			description: "Transform hours of design work into minutes of content input. Our grid-based system delivers professional results at the speed of thought."
		},
		{
			title: "Quality obsession",
			description: "We believe presentations should be presentation-worthy. Every template, every layout, every detail is crafted to make you look exceptional."
		}
	];
</script>

<SecondaryHero
	title="Design-forward by default"
	subtitle="AI formatting that thinks like you"
	imageSrc="/generated/image-natural-light-candid-photograph-of-a-div.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- Founder Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet our founder."
	subtitle="Building the future of presentations."
	stakeholders={[
		{
			name: "Leo Radloff",
			position: "Founder",
			bio: "Transforming presentation creation from hours of design work into minutes of content input through AI-powered grid layouts.",
			image: "/generated/image-professional-headshot-of-a-business-foun.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to transform your presentations?"
	subtitle="Join the design revolution"
	description="Stop wasting hours on PowerPoint. Join marketing managers at fast-growing SaaS companies who create pitch-perfect presentations in minutes, not hours."
	imageSrc="/generated/image-photorealistic-editorial-corporate-lifes.webp"
/>
