<script>
   import TimelineOrgCard from '$lib/components/TimelineOrgCard.svelte';
	import TimelineActivity from '$lib/components/TimelineActivity.svelte';
    // Define data for TimelineOrgCard
    const orgCards = [
      {
        logo: '/logo1.png',
        name: 'Duggup',
        location: 'San Francisco Bay Area',
        joined: 'Nov 2022',
        designation: 'Co-Founder and CEO',
        type: 'Full-time · Remote'
      },
      {
        logo: '/logo2.jpeg',
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
        content: 'No amount of technology can convert a bad story into a good story.',
        cards: [
          {
            imageSrc: '/card1.jpeg',
            altText: 'Card 1',
            content: 'No amount of technology can convert a bad story into a good story.'
          },
          {
            imageSrc: '/card2.jpeg',
            altText: 'Card 2',
            content: 'Most people don\'t have original ideas. Here is how Sam Altman pushes...'
          }
        ]
      },
      {
        date: 'Dec, 2023',
        content: 'Startup Lesson I am reflecting. Don\'t build for the "average person".',
        cards: [
          {
            imageSrc: '/card3.jpeg',
            altText: 'Card 3',
            content: 'Startup Lesson I am reflecting. Don\'t build for the "average person".'
          },
          {
            imageSrc: '/card4.png',
            altText: 'Card 4',
            content: 'Your biggest regrets at 80 will be acts of omission.'
          }
        ]
      }
    ];
  </script>
  
  <section class="relative">
    {#each activities as { date, content, cards }}
      <TimelineActivity {date} {content} {cards} />
    {/each}
  
    {#each orgCards as { logo, name, location, joined, designation, type }}
      <TimelineOrgCard
        {logo}
        {name}
        {location}
        {joined}
        {designation}
        {type}
      />
    {/each}
  </section>
  