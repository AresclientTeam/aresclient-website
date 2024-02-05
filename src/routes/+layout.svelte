<script>
  import "../app.pcss";

  import "aos/dist/aos.css";
  // @ts-ignore
  import AOS from "aos";

  import { onMount } from "svelte";

  onMount(() => {
    AOS.init();
  });
</script>

<div class="dark">
  <slot />
</div>
