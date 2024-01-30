<!-- CardGrid.svelte -->
<script lang="ts">
  import Card from "./Card.svelte";

  const cards = [
    {
      title: "Cosmetics",
      description: "We offer a variety of beautiful cosmetics for our users.",
    },
    {
      title: "Noteworthy technology acquisitions 2021",
      description:
        "Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.",
    },
    {
      title: "Noteworthy technology acquisitions 2021",
      description:
        "Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.",
    },
    {
      title: "Noteworthy technology acquisitions 2021",
      description:
        "Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.",
    },
    // Add more cards as needed
  ];
</script>

<section class="bg-white dark:bg-gray-900 pt-32 flex content-center">
  <div class="grid grid-cols-5 gap-3">
    {#each cards as { title, description } (title)}
      <Card {title} {description} />
    {/each}
  </div>
</section>
