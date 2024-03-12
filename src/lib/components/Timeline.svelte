<script>
	import TimelineOrgCard from '$lib/components/TimelineOrgCard.svelte';
	import TimelineActivity from '$lib/components/TimelineActivity.svelte';
	// Define data for TimelineOrgCard
	const orgCards = [
		{
			logo: 'https://s3-alpha-sig.figma.com/img/f1bc/3eca/3db6ec41cda31968010a7f56f3c3658a?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=k3FJIC-SLr3EdRrkSLuszhDsVyH9BVEPNdw5aBS~1SPEtzWrbt40iKzcfTAR1ryG4rkUsWdo1lbGVdvTrOOaOjxLgaDlHv~-5MQ82x0SLHenZsDIN5uKYQOjiY69SgI8oisyKBYitaOiIuDChDPQ1DQjqHJ11M2eSPtlZbHIHStHDoB7pju31u0JsL5ddhFmkKWLxoyjHraMQjCJpLJrMjI2GwD9A9M3vwbi2UtoIpljPs8jal1NuBb0AwqDMmqwT~nPeOiMUIjNDht01JhLaSBN8z6mvWWsyeNRNExS01geQ8JzBUQ~jW5SK8b~yz2g2T7XaS2yN0V9fRVp~-QIHw__',
			name: 'Duggup',
			location: 'San Francisco Bay Area',
			joined: 'Nov 2022',
			designation: 'Co-Founder and CEO',
			type: 'Full-time · Remote'
		},
		{
			logo: 'https://s3-alpha-sig.figma.com/img/1b23/f02f/60bc556cd22a575549ce43ad307ec0ee?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=OS-m9FouegWKOM0bIXP3XHmNqAB0ujry7al3wNrJ7uDCQM1IpwT5bfZIeFLavdbEq10jvOKSCszEaAUdkObTfroVRK5bAhjiLykRRrmGpRJtDYUxb4L7E2FdeXGcD9LMeBlA6d-oOIhvj7z9ERRNnmA6R4GmsTRe~KoVSP23zk0O~73I~pmAeJHJu4kCyncpqHl5RRssd3XrUZyYELuGj01U5Z0zoinaRwa14DHoLFIIIwKUluIkKQhLUuLhay3kZ9wx5ymanxzFMC6A766bZavoSVvOnNDkADuQ9Whozaqi5pZ9nAgxjy19kw2vckjhOGw0CvZ0BUA0lrroIGGQjw__',
			name: 'BetterUp',
			location: 'San Francisco Bay Area',
			joined: 'Sep 2022',
			designation: 'VP Engineering',
			type: 'Full-time'
		}
	];

	// Define data for TimelineActivity
	const activities = [
		{
			date: 'Dec, 2023',
			cards: [
				{
					imageSrc:
						'https://s3-alpha-sig.figma.com/img/ccdc/bd9b/5b2f7dca180260dd9a121e21e4ccb158?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=ZlSaApWAaRGs-9-eJpkITxEY8gIsdP2RmwcwIrTdyMCX8AJw~ZrkOLecj1DvkNt8k6jzE1Kq4E3Ru3RAO6jimGMmZGlRTWTh7rbRPbo0eH5TK7dKet8dkp9OHVksPDJvE2CXPjo-3fzFrw9mnvlBquyc4Mpp6crIkK5mLP2Qug6WaZ6AxcKYEQeOV2iq3XD1O70se3E7QQDTjamICNQ2G5-Lyi7Kz80Jju4uHmuis3d18Ym8TG9-UndhuOQvG2ucRakuPY1lxBs4u9OR3U76SKpAcQdOAQi6ceHMWXIohteueH9aw-9QrrGbKBs2kGW2xv5fuNOzAo~ow~BzlUlZmw__',
					altText: 'Card 1',
					content: 'No amount of technology can convert a bad story into a good story.'
				},
				{
					imageSrc:
						'https://s3-alpha-sig.figma.com/img/25ac/166c/37888417ccf24a1991743ef364aea246?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=XM0c80roF5Rb7lR3GOYcI24mWP3jQfVCuVUiGlJYZ5823~QveSguwSz8wkMGvfpSZTVYbplRzCfamcEx7WlDi7NnCqV~gU67eGDIuxD-RJyd4bm~g09ZC1MukaQJ5hnexd7ZPYYW5Lra4rcn1Y1-JfFlibJ92U7IFs9NCuv~K~Z3HE-1UO7A7bPr1nWLsDMefZDxFVN88~O1E12P2uME8uniK-5P5bRrKuWxfjdMDoM6jP7PHcvgeYre-EnZqEmw-bUwi~FUTMDw73x8wlFk0gePQhLSV7DBrMddj15323vb3opwfEDZrYRO4wSNbTYZ-wpSKL4Z2UKLoSrS9Tf0kg__',
					altText: 'Card 2',
					content: "Most people don't have original ideas. Here is how Sam Altman pushes..."
				}
			]
		},
		{
			date: 'Dec, 2023',
			cards: [
				{
					imageSrc:
						'https://s3-alpha-sig.figma.com/img/19af/a12d/f27e595212d7ad397a130cdeb8ac6c5e?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=co3FZnG~yZ0IFJXw-HS-y8jQ00ky~q5O~N83Vv8nv2lF9quL8ofhrhBCS3DJQbgsk7gWwtztJR1RkaHU-dU~cphQiH~Mz167wx1VaLkripHxCAnFPVaQLjcP9OneAdKi4A5T304hWBaysdZDnp7ipOqbVqOeSnWWuns0o0hSpu54RZxGeRHhdI2hQOwTvxt88F4pgA-eMehgVZ~PElkhkVoP06aLkzcE3QE8FRl4kYowwzhz6OB~~QzwJyk1wMv3Sf3WD89vS47eahjVT91n-0DxscfWKdtNpRB124nOHuhNE3MRBfq8TvuLcFRIxtDGV5OgviF8zTh9dhi4plTQAA__',
					altText: 'Card 3',
					content: 'Startup Lesson I am reflecting. Don\'t build for the "average person".'
				},
				{
					imageSrc:
						'https://s3-alpha-sig.figma.com/img/fcaf/84e6/4461b5caa81a8f3d2afecfa15491ed1f?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=MhDkZ4HZO98DAsxAu0-UGj2XCSsOJ5~ZfrKBIWz~ecEe2dKv8X2KVFpBdj9Jv4B4qxjivX7gkI5XRIAo-LISqj0yhStNv0GSqf-2pNusTMuWL67OBbA-T-D79r5aMv0Bixx7U9Lu-oHqC-fsBYBvZyatLNbzJcEHrEJK3ssvQ6dqSCW9MrrTVy74lN7FkdXe~M-FaMW8AB0D7RSW-uh~7esb8wOwaV-uGodh6jGi9FCyaoXR7F9gc6x8tyxsqTqpCu-MXUV1TR0i0l2ttXDF0tk0UF9M5MZF7k6GGsInY01qMGq7YjvdTsDNOaE0HEswFLYVycOlvHndNotm0852bA__',
					altText: 'Card 4',
					content: 'Your biggest regrets at 80 will be acts of omission.'
				}
			]
		}
	];
</script>

<section class="relative">
	{#each activities as { date, cards }, i}
		{#if i === 0}
			<TimelineActivity {date} {cards} />
		{/if}
	{/each}

	{#each orgCards as { logo, name, location, joined, designation, type }, i}
		{#if i === 0}
			<TimelineOrgCard {logo} {name} {location} {joined} {designation} {type} />
		{/if}
	{/each}

	{#each activities as { date, cards }, i}
		{#if i === 1}
			<TimelineActivity {date} {cards} />
		{/if}
	{/each}

	{#each orgCards as { logo, name, location, joined, designation, type }, i}
		{#if i === 1}
			<TimelineOrgCard {logo} {name} {location} {joined} {designation} {type} />
		{/if}
	{/each}
</section>
