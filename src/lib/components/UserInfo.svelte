<script>
	import { Button } from '$lib/components/ui/button';
	import * as Avatar from '$lib/components/ui/avatar';
</script>

<div class="mx-auto mt-12 flex w-4/5 flex-col items-center justify-around md:flex-row">
	<div class="flex min-w-[120px] flex-col items-center justify-center">
		<Avatar.Root class="h-[120px] w-[120px] border-2 border-solid border-gray-200 ">
			<Avatar.Image
				src="https://s3-alpha-sig.figma.com/img/8ed8/92f8/c135d62b39e8cc0f1e2dfce61ea32106?Expires=1711324800&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=jdQX-2LIKd-iagc6n2olzrfdMwFrAKHBFqk4aW4fS2nOOe5pZjnRgGH94~XA5qQp0IMD7P83u45zu~dH5h-a1wFU2XCJxGRVMyC7AaAYg-UCYnXJYqetzzcoxPmXV178gzY3e0eUlpO8HSBIlhK91S3vCW4sA1dU2P9Ttxmyb4gDf112piLShysBuofSPVUglEgZj4XESShQ2PAIegY-pJrAyF4HT5lGy0tePo8IzINqBuT40vKgZ4~0j-gVvSyUMHof8zneTvepnwCKlPln1BshDJVxP3XzNZuUBdXxgfRVCGl2x8ZCPiahMZzKjdi3VDI~lKGachykK~cA2KAm6Q__"
				alt="avatar"
			/>
			<Avatar.Fallback>KK</Avatar.Fallback>
		</Avatar.Root>
		<h1 class="text-center text-xl font-bold text-gray-500">Krishna <br /> Kiran</h1>
	</div>
	<div class="flex flex-col items-center justify-between gap-3">
		<div class="flex flex-row items-center justify-between gap-8">
			<p class="max-w-sm text-sm text-black">
				Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
				Engineering. I write hot-takes on building a business, shipping delightful products and
				accelerating product and career growth.
			</p>
			<div class="flex flex-col items-end justify-end">
				<img src="./LogoIcon.svg" alt="logo" class="w-[36px] rounded-full" />
				<p class="font-bold">Duggup</p>
				<p class="text-sm text-[#7A9299]">Co-Founder and CEO</p>
			</div>
		</div>
		<div class="flex w-full flex-row items-center justify-between">
			<Button variant="default">Following</Button>
			<div class="flex flex-row items-center">
				<a href="https://github.com/harshpathakzz" target="_blank">
					<Button variant="link" size="sm" class="gap-2">
						<p>My website</p>
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.20156 1.59961H4.00156C2.67608 1.59961 1.60156 2.67413 1.60156 3.99961V11.9997C1.60156 13.3252 2.67608 14.3997 4.00156 14.3997H12.0016C13.327 14.3997 14.4016 13.3252 14.4016 11.9997V8.79961M10.4012 1.5998L14.4016 1.59961M14.4016 1.59961V5.19971M14.4016 1.59961L7.60098 8.39942"
								stroke="#4D4D4D"
								stroke-width="1.5"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
					</Button>
				</a>
				<Button variant="link" size="sm">
					<svg
						width="24"
						height="6"
						viewBox="0 0 24 6"
						fill="none"
						xmlns="http://www.w3.org/2000/svg"
					>
						<path
							d="M4.90078 2.99922C4.90078 3.71719 4.31875 4.29922 3.60078 4.29922C2.88281 4.29922 2.30078 3.71719 2.30078 2.99922C2.30078 2.28125 2.88281 1.69922 3.60078 1.69922C4.31875 1.69922 4.90078 2.28125 4.90078 2.99922ZM13.3008 2.99922C13.3008 3.71719 12.7188 4.29922 12.0008 4.29922C11.2828 4.29922 10.7008 3.71719 10.7008 2.99922C10.7008 2.28125 11.2828 1.69922 12.0008 1.69922C12.7188 1.69922 13.3008 2.28125 13.3008 2.99922ZM21.7008 2.99922C21.7008 3.71719 21.1188 4.29922 20.4008 4.29922C19.6828 4.29922 19.1008 3.71719 19.1008 2.99922C19.1008 2.28125 19.6828 1.69922 20.4008 1.69922C21.1188 1.69922 21.7008 2.28125 21.7008 2.99922Z"
							stroke="#A5B9D3"
							stroke-width="3"
						/>
					</svg>
				</Button>
			</div>
		</div>
	</div>
</div>
