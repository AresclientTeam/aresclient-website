<script>
  import CardGrid from "./components/CardGrid.svelte";
  import Features from "./components/Features.svelte";
  import Footer from "./components/Footer.svelte";
  import LearnMore from "./components/LearnMore.svelte";
  import Navbar from "./components/Navbar.svelte";
</script>

<Navbar />

<LearnMore />

<Features />

<CardGrid />

<div
  class="fixed bottom-1 flex justify-center items-center left-[50%] translate-x-[-50%]"
>
  <Footer />
</div>
