<script>
	let openIndex = 0;
	const faqs = [
		{
			question: "Who can use HiPeople?",
			answer: "HiPeople is built for talent acquisition teams and hiring managers. Whether you're a high-growth startup or a global enterprise, our platform scales to meet your screening and assessment needs. We work with 2,000+ teams worldwide."
		},
		{
			question: "Can I try HiPeople for free?",
			answer: "Yes! We offer a free trial so you can experience our AI screening, assessments, and reference checks firsthand. No credit card required to get started."
		},
		{
			question: "How does the AI screening work?",
			answer: "Our AI analyzes candidate applications and can even conduct automated screening calls. It evaluates real signals like skills and experience against your job requirements, providing a ranked shortlist of best-fit candidates."
		},
		{
			question: "Is HiPeople compliant with data protection laws?",
			answer: "Absolutely. We are fully GDPR and CCPA aligned, and maintain SOC 2–type security controls. We also provide independent AI audit reports via Warden AI to ensure transparency and fairness."
		},
		{
			question: "Does it integrate with my ATS?",
			answer: "Yes, HiPeople integrates with all leading applicant tracking systems including Greenhouse, Lever, Workday, Ashby, and many more. We act as an augmentation layer on top of your existing workflow."
		},
		{
			question: "What languages do you support?",
			answer: "We offer localized support for English, Spanish, German, and Portuguese across our website and product surfaces."
		}
	];
</script>

<section class="py-24">
	<div class="mx-auto max-w-[1400px] px-6">
		<div class="grid grid-cols-1 gap-16 lg:grid-cols-12">
			<!-- Left Side -->
			<div class="lg:col-span-4">
				<div class="mb-4 text-[10px] font-bold tracking-widest text-gray-500 uppercase">[06] FAQ</div>
				<h2 class="mb-6 text-4xl font-medium tracking-tight text-gray-900">Your questions, answered</h2>
				<p class="mb-8 text-lg leading-relaxed text-gray-600">
					We're here to help. Reach out to our team for guidance on how to integrate HiPeople into your hiring workflow.
				</p>
				<a href="#" class="inline-block bg-gray-900 px-6 py-3 text-[11px] font-bold tracking-widest text-white transition-colors hover:bg-gray-800 uppercase">
					Book a Demo
				</a>
			</div>

			<!-- Right Side (Accordion) -->
			<div class="lg:col-span-8">
				<div class="divide-y divide-gray-200 border-t border-b border-gray-200">
					{#each faqs as faq, i}
						<div class="group">
							<button 
								class="flex w-full items-center justify-between py-6 text-left focus:outline-none"
								onclick={() => openIndex = openIndex === i ? -1 : i}
							>
								<span class="text-lg font-medium text-gray-900">{faq.question}</span>
								<span class="ml-4 flex h-6 w-6 items-center justify-center text-gray-400">
									{#if openIndex === i}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 6L6 18M6 6l12 12"/></svg>
									{:else}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
									{/if}
								</span>
							</button>
							{#if openIndex === i}
								<div class="pb-6 text-gray-600 leading-relaxed">
									{faq.answer}
								</div>
							{/if}
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>