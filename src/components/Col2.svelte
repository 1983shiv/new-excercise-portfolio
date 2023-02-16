<script>
    export let imgsrc;
    export let title;
    export let desc;
</script>

<section class="text-gray-600 body-font">
    <div class="container mx-auto flex px-5 py-6 md:flex-row flex-col items-center">
      <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 mb-10 md:mb-0">
        <img class="object-cover object-center rounded" alt="hero" src={imgsrc}>
      </div>
      <div class="lg:flex-grow md:w-1/2 lg:pl-24 md:pl-16 flex flex-col md:items-start md:text-left items-center text-center">
        <h1 class="title-font sm:text-4xl text-3xl mb-4 font-medium text-gray-900">{title}
        </h1>
        <p class="mb-8 leading-relaxed">{desc}</p>
        <div class="flex justify-center">
            <button class="inline-flex font-bold bg-orange-600 text-white border-0 py-2 px-6 focus:outline-none  rounded text-lg">Ask for Quick Quote</button>
          
        </div>
      </div>
    </div>
  </section>