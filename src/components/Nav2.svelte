<script>
  // Menu Source: https://github.com/justalever/tailwind-navbar/blob/master/public/index.html
  import { goto } from "$app/navigation"
  import Navli from "../components/Navli.svelte";
  import Logo from "../components/Logo.svelte";
  export let isOpen = true;

  function toggleNav() {
    isOpen = !isOpen;
  }

  function funcKeyPress(event) {
    if (event.key === 'Enter' || event.key === ' ') {
      handleClick();
    }
  }
</script>

<header
  class="lg:px-16 px-6 bg-shades-50 flex flex-wrap items-center lg:py-2 py-2"
>
  <Logo />

  <label
    for="menu-toggle"
    class="pointer-cursor lg:hidden block"
    on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}
    ><svg
      class="fill-current text-shades-900"
      xmlns="http://www.w3.org/2000/svg"
      width="20"
      height="20"
      viewBox="0 0 20 20"
      ><title>menu</title><path
        d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"
      /></svg></label>
    <input class={isOpen ? "hidden" : ""} type="hidden" id="menu-toggle" />

  <div
    class="{isOpen ? 'hidden' : ''} lg:flex lg:items-center lg:w-auto w-full"
    id="menu"
  >
    <nav>
      <ul
        class="lg:flex items-center justify-between text-base text-shades-700 pt-4 lg:pt-0"
      >
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Home</a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Custom T-Shirts
          </a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Printing Techniques
          </a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Locations
          </a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Case Studies
          </a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:p-4 py-3 px-0 block border-b-2 font-2xl border-transparent hover:border-main-400"
            href="/">Blog
          </a>
        </li>
        <li on:click={toggleNav} on:keypress={(event) => funcKeyPress(event)}>
          <a
            class="lg:px-4 lg:py-2 py-2 px-0 block font-bold bg-orange-600 rounded-md text-white border-transparent hover:border-main-400 hover:bg-slate-200 hover:text-orange-600"
            href="/">Get a Quote
          </a>
        </li>
      </ul>
    </nav>
  </div>
</header>
