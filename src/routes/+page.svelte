<script lang="ts">
	import Button from '$lib/components/ui/button/button.svelte';
	import Nav from '$lib/components/ui/nav.svelte';
	import UserInfo from '$lib/components/UserInfo.svelte';
	import TimelineOrgCard from '$lib/components/TimelineOrgCard.svelte';
	import TimelineActivity from '$lib/components/TimelineActivity.svelte';
	import Timeline from '$lib/components/Timeline.svelte';
</script>

<div>
	<Nav />
	<UserInfo />
	<!-- <TimelineOrgCard />
	<TimelineActivity
		date="March 11, 2024"
		cards={[
			{
				imageSrc: '/card1.jpeg',
				altText: 'Card 1',
				content: 'Content for card 1'
			},
			{
				imageSrc: '/card2.jpeg',
				altText: 'Card 2',
				content: 'Content for card 2'
			},
			{
				imageSrc: '/card3.jpeg',
				altText: 'Card 3',
				content: 'Content for card 3'
			}
		]}
	/> -->
	<Timeline />
</div>
