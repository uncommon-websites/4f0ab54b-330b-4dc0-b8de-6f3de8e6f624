<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Create decks without the design struggle"
	subtitle="Slides formats your content beautifully. Every time."
	imageSrc="/generated/image-professional-manager-presenting-confiden.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by industry leaders" 
	logoUrls={[
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/figma.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/linear.app/w/400/h/400/logo'
	]}
/>

<Summary
	title="Presentations without the pain"
	text="Slides takes the frustration out of presentation design for marketing teams at fast-growing SaaS companies. Just add your content—our AI-powered grid system handles the layout, branding, and formatting automatically. Save 8+ hours per deck with layout automation that thinks like a designer, not generic templates."
/>

<Testimonials
	testimonials={[
		{
			name: "Clara Reyes",
			position: "Head of Marketing",
			company: "Able.io",
			quote:
				"We used to spend 8 hours building a deck. With Slides, we ship in under 45 minutes—with better design.",
			image: "/generated/image-professional-corporate-headshot-of-a-con.webp"
		},
		{
			name: "Kenji Okafor",
			position: "Marketing Lead",
			company: "LambdaStack",
			quote:
				"Slides helped our team cut design requests by 80%. Now we move way faster and stay on brand every time.",
			image: "/generated/image-professional-corporate-headshot-of-a-con.webp"
		},
		{
			name: "Alya Tanaka",
			position: "Growth Marketer",
			company: "Intuitiv",
			quote:
				"We saved $12K in design contractor fees last quarter thanks to Slides. It just works.",
			image: "/generated/image-professional-corporate-headshot-of-a-con.webp"
		}
	]}
/>

<Features
	title="Why marketing teams choose Slides"
	subtitle="Transform your pitch deck workflow from frustrating to effortless"
	features={[
		{
			title: "Grid-based AI that thinks like designers",
			description: "Our revolutionary grid system automatically formats content with perfect spacing and alignment. No more wrestling with slide layouts.",
			imageSrc: "/generated/image-natural-light-design-studio-candid-34-an.webp"
		},
		{
			title: "Brand consistency across every slide",
			description: "Preserve your company's visual identity with intelligent brand recognition. Your presentations look professionally designed, never generic.",
			imageSrc: "/generated/image-bright-creative-studio-overhead-top-down.webp"
		},
		{
			title: "8+ hours saved per presentation",
			description: "What used to take all day now takes minutes. Focus on content strategy while Slides handles the design work.",
			imageSrc: "/generated/image-design-studio-dynamic-angle-fast-paced-w.webp"
		},
		{
			title: "Designer-quality output, every time",
			description: "Professional layouts that rival expensive design agencies. Your team delivers pitch-perfect presentations that impress investors.",
			imageSrc: "/generated/image-architectural-boardroom-medium-wide-prof.webp"
		},
		{
			title: "Investor-ready templates built for SaaS",
			description: "Skip the guesswork with proven pitch deck structures. Templates designed specifically for Series A-C funding rounds.",
			imageSrc: "/generated/image-sunlit-conference-room-wide-shot-a-prese.webp"
		},
		{
			title: "Real-time collaboration that scales",
			description: "Your entire marketing team can contribute simultaneously. Changes sync instantly without version control chaos.",
			imageSrc: "/generated/image-modern-co-working-space-medium-shot-a-di.webp"
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Stop wasting time on slide layouts"
	subtitle="Start creating presentations that impress"
	description="Join thousands of marketing teams who've already transformed their presentation workflow. Get from content to compelling pitch deck in under 45 minutes—with professional design that preserves your brand identity."
	imageSrc="/generated/image-photorealistic-editorial-corporate-portr.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Start creating now",
			variant: "primary"
		},
		{
			href: "/demo",
			label: "See it in action",
			variant: "secondary"
		}
	]}
/>
