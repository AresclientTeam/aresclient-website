<script>
  import CardGrid from "./components/CardGrid.svelte";
  import Features from "./components/Features.svelte";
  import Footer from "./components/Footer.svelte";
  import LearnMore from "./components/LearnMore.svelte";
  import Navbar from "./components/Navbar.svelte";
</script>

<Navbar />

<LearnMore />
<hr class="bg-text" />

<Features />

<hr class="bg-text" />

<CardGrid />

<div
  class="sm:fixed bottom-1 flex justify-center items-center sm:left-[50%] sm:translate-x-[-50%]"
>
  <Footer />
</div>
