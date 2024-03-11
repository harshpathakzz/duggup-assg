<script lang="ts">
	import * as Card from '$lib/components/ui/card';
	export let imageSrc: string;
	export let altText: string;
	export let content: string;
</script>

<div>
	<Card.Root class="max-w-[350px] rounded-xl">
		<Card.Header class="m-0 p-0">
			<img src={imageSrc} alt={altText} class="h-[150px] max-w-[350px] rounded-t-xl object-cover" />
		</Card.Header>
		<Card.Content>
			<p class="mt-5 text-sm font-light text-black">{content}</p>
		</Card.Content>
	</Card.Root>
</div>
