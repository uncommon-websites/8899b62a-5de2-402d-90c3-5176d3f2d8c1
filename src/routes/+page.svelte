<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";

	// Icons
	import IconDollarSign from "~icons/lucide/dollar-sign";
	import IconLeaf from "~icons/lucide/leaf";
	import IconZap from "~icons/lucide/zap";
	import IconShield from "~icons/lucide/shield";
	import IconArrowUpDown from "~icons/lucide/arrow-up-down";
	import IconGauge from "~icons/lucide/gauge";
</script>

<CenteredTextOnlyHero
	title="Faster compute. Lower cost. No strings."
	subtitle="Run your LLM workloads at massive scale—without vendor lock-in or runaway bills. Transparent pricing, green-powered infrastructure, and month-to-month contracts that flex with your needs."
	imageSrc="/generated/image-a-modern-office-environment-with-a-team-.webp"
/>
<LogoScroller
	label="Trusted by AI pioneers"
	logoUrls={[
		'https://cdn.brandfetch.io/openai.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/anthropic.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/huggingface.co/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stability.ai/w/400/h/400/logo'
	]}
/>

<Summary
	title="Enterprise AI compute, reimagined"
	text="Consensus Core delivers direct access to H100 GPU clusters for AI research teams who need to train large language models without burning through runway on legacy cloud providers. We operate green-powered datacenters that eliminate third-party markup, delivering 80% cost savings and up to 35X faster performance—with flexible month-to-month contracts that scale from 8 to 4,088 GPUs as your experiments evolve."
/>

<Testimonials
	testimonials={[
		{
			name: "Dr. Kenji Yamamoto",
			position: "VP of AI Infrastructure",
			company: "Cerebral Labs",
			quote:
				"We cut our H100 costs by 73% and eliminated the AWS queue entirely. Our GPT training runs that used to cost $180K now run for under $50K—same performance, zero vendor lock-in. Consensus Core gave us 12 months of extra runway.",
			image: "/generated/image-portrait-of-a-professional-asian-male-en.webp"
		},
		{
			name: "Amara Okonkwo",
			position: "Head of ML Engineering",
			company: "Vantage Intelligence",
			quote:
				"Month-to-month contracts saved us from a $2M annual commitment we couldn't afford. We scaled from 8 to 248 GPUs in 48 hours without renegotiating terms. The transparent per-hour pricing meant no surprises—just predictable costs that our CFO actually approved.",
			image: "/generated/image-portrait-of-a-professional-african-ameri.webp"
		},
		{
			name: "Marcus Lindström",
			position: "Chief Research Officer",
			company: "Axiom Dynamics",
			quote:
				"Three months of Azure queues killed our experiment velocity. With Consensus Core's direct GPU access, we train models 35X faster and iterate daily instead of weekly. Time to market dropped from 9 months to 4—that's the difference between leading and following.",
			image: "/generated/image-portrait-of-a-professional-caucasian-mal.webp"
		}
	]}
/>

<Features
	title="Built for AI teams who demand more"
	subtitle="Enterprise-grade infrastructure that eliminates the compromises between cost, performance, and sustainability"
	features={[
		{
			title: "80% lower costs than legacy clouds",
			description:
				"Direct datacenter access eliminates third-party markup and delivers transparent per-hour pricing from $2.15/GPU. No hidden fees, no budget surprises—just predictable costs that preserve your runway while you scale.",
			icon: IconDollarSign
		},
		{
			title: "100% green-powered infrastructure",
			description:
				"Train your models on renewable energy without compromising performance. Our gigawatt-scale green power sites deliver the compute you need with the environmental responsibility your stakeholders expect.",
			icon: IconLeaf
		},
		{
			title: "Direct GPU access, zero markup",
			description:
				"Connect directly to H100 clusters with 3,200 Gbps Infiniband networking. Our datacenter economics mean you pay for compute, not corporate overhead—giving you enterprise performance at startup prices.",
			icon: IconZap
		},
		{
			title: "NVIDIA Preferred Elite Partner",
			description:
				"Early access to Blackwell GPU reservations and state-of-the-art NVIDIA networking infrastructure. Partner with a team that has direct lines to the hardware shaping AI's future.",
			icon: IconShield
		},
		{
			title: "Scale from 8 to 4,088 GPUs without renegotiation",
			description:
				"Month-to-month contracts that flex with your experiments. Start with a small cluster, scale to supercomputer configurations—all with transparent pricing and zero vendor lock-in.",
			icon: IconArrowUpDown
		},
		{
			title: "35X faster than legacy providers",
			description:
				"Optimized end-to-end architecture eliminates queue delays and delivers peak performance for LLM training. Run more experiments, iterate faster, and ship breakthrough models while competitors wait in line.",
			icon: IconGauge
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Stop burning runway on cloud bills"
	subtitle="Start training on your terms"
	description="Every week on AWS costs you another 80% in markup. Month-to-month contracts mean you can switch tomorrow—no penalties, no negotiations, no risk. Get transparent H100 pricing and see exactly how much runway you'll reclaim."
	imageSrc="/generated/image-a-confident-researcher-sitting-at-a-mode.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Get transparent pricing",
			variant: "primary"
		},
		{
			href: "/contact",
			label: "Talk to our team",
			variant: "secondary"
		}
	]}
/>
