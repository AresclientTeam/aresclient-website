<script>
  import "../app.pcss";

  import "aos/dist/aos.css";
  // @ts-ignore
  import AOS from "aos";

  import { onMount } from "svelte";
  console.log("AOS imported");

  onMount(() => {
    console.log("AOS intializing");
    AOS.init();
    console.log("AOS initialized");
  });
</script>

<div class="dark">
  <slot />
</div>
