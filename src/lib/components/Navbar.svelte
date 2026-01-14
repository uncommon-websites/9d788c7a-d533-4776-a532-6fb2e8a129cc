<script>
	// Navbar
</script>

<div class="sticky top-0 z-50 w-full bg-white">
	<!-- Top Banner -->
	<div class="bg-black px-4 py-2 text-center text-[11px] font-medium tracking-wide text-white">
		<a href="#" class="hover:underline">
			HiPeople is trusted by 2,000+ hiring teams worldwide &rarr; See why
		</a>
	</div>

	<!-- Main Navigation -->
	<nav class="border-b border-gray-200 px-6 py-4">
		<div class="mx-auto flex max-w-[1400px] items-center justify-between">
			<!-- Logo and Left Links -->
			<div class="flex items-center gap-12">
				<a href="/" class="text-xl font-bold tracking-tight text-gray-900">
					HiPeople
				</a>
				
				<div class="hidden items-center gap-8 md:flex">
					{#each ['Product', 'Solutions', 'Resources', 'Pricing'] as item}
						<a href="#" class="flex items-center gap-1 text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
							{item}
							{#if item === 'Product' || item === 'Resources' || item === 'Solutions'}
								<svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="opacity-50"><path d="m6 9 6 6 6-6"/></svg>
							{/if}
						</a>
					{/each}
				</div>
			</div>

			<!-- Right Actions -->
			<div class="flex items-center gap-6">
				<a href="#" class="text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
					Sign In
				</a>
				<a href="#" class="text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
					Book a Demo
				</a>
				<a href="#" class="bg-gray-900 px-4 py-2 text-[11px] font-bold tracking-widest text-white transition-colors hover:bg-gray-800 uppercase">
					Try for Free
				</a>
			</div>
		</div>
	</nav>
</div>