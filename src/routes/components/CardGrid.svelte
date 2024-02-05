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

<section class="bg-white dark:bg-background py-32 flex">
  <div class="py-8 px-4 mx-auto max-w-screen-xl sm:py-16 lg:px-6 items-center">
    <div
      class="grid grid-cols-auto-300 gap-3 content-center"
      data-aos="zoom-in"
    >
      {#each cards as { title, description } (title)}
        <Card {title} {description} />
      {/each}
    </div>
  </div>
</section>
