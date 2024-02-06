<script>
  import {
    NavBrand,
    NavHamburger,
    NavLi,
    NavUl,
    Navbar,
  } from "flowbite-svelte";
  import MediaQuery from "./MediaQuery.svelte";
</script>

<Navbar class="bg-background dark:bg-background">
  <NavBrand href="/">
    <img src="logo_white.png" class="me-3 h-6 sm:h-9" alt="Ares Logo" />
    <span
      class="self-center whitespace-nowrap text-xl font-semibold dark:text-text"
      >Ares</span
    >
  </NavBrand>
  <div class="flex md:order-2 dark:text-text">
    <a
      href="/download"
      class="inline-flex items-center justify-center px-5 py-2 text-base font-medium text-center text-text border border-primary rounded-lg hover:bg-text focus:ring-4 focus:ring-text dark:text-text dark:border-secondary dark:hover:bg-secondary dark:focus:ring-accent"
      data-aos="zoom-in"
    >
      Download
    </a>
    <NavHamburger menuClass="dark:hover-backgroundSecondary" />
  </div>
  <MediaQuery query="(min-width: 640px)" let:matches>
    {#if matches}
      <NavUl class="order-1">
        <NavLi
          nonActiveClass="text-textDark hover:text-text"
          href="/"
          active={true}>Home</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/about"
          >About</NavLi
        >
        <NavLi
          nonActiveClass="text-textDark hover:text-text"
          href="/docs/components/navbar">Navbar</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/pricing"
          >Pricing</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/contact"
          >Contact</NavLi
        >
      </NavUl>
    {:else}
      <NavUl
        class="order-1"
        ulClass="dark:bg-backgroundSecondary dark:border-background"
      >
        <NavLi
          nonActiveClass="text-textDark hover:text-text"
          href="/"
          active={true}>Home</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/about"
          >About</NavLi
        >
        <NavLi
          nonActiveClass="text-textDark hover:text-text"
          href="/docs/components/navbar">Navbar</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/pricing"
          >Pricing</NavLi
        >
        <NavLi nonActiveClass="text-textDark hover:text-text" href="/contact"
          >Contact</NavLi
        >
      </NavUl>
    {/if}
  </MediaQuery>
</Navbar>
