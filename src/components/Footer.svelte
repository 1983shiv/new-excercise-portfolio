<script context="module">
  import Logo from "./Logo.svelte";
	import SocialFooter from "./SocialFooter.svelte";
</script>


<footer class="bg-shades-100 mb-0">
  <div class="flex flex-wrap px-12 py-5 items-center justify-center">
    <a
      href="."
      class="title-font font-medium text-shades-900"
    >
    <img class="object-cover object-center rounded" width="160" height="auto" alt="hero" src="./logo-lastminutetshirtprinting-dark.png" >

    </a>
    <p
    class="text-sm text-shades-900 ml-4 sm:border-shades-200"
  >
    All right reserved!
  </p>
    <div class="flex mb-4 ml-4 text-right">
      <SocialFooter />
    </div>
  </div>
</footer>
