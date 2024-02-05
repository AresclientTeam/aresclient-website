<script lang="ts">
  export let title: any;
  export let description: any;
</script>

<a
  class="block bg-white border border-primary rounded-lg shadow hover:bg-gray-100 dark:bg-backgroundSecondary dark:border-primary dark:hover:bg-secondary"
>
  <h5
    class="mx-2 my-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-text"
  >
    {title}
  </h5>
  <p class="mx-2 my-2 font-normal text-gray-700 dark:text-gray-400">
    {description}
  </p>
</a>
