<script>
    import "./app.css";

    function scrollToTop(){
    document.documentElement.scrollTo({
      top: 0,
      behavior:"smooth",
    });
  }
  function expand() {
 
  }
  </script>
  <main class="bg-bgblack h-full text-white">


  <nav class="m-0 p-0 h-10 items-center w-full flex place-content-evenly bg-stone-900 text-white flex-row ">
    <a class=" w-24 rounded-lg text-center bg-stone-800 hover:bg-stone-700" href="/homepage">Hjem</a>
    <a class=" w-24 rounded-lg  text-center bg-stone-800 hover:bg-stone-700"  href="/tutorial">Tutorial</a>
    <!-- <a class=" w-24 rounded-lg  text-center bg-stone-800 hover:bg-stone-700"  href="/contactme">Kontak oss</a> -->
  </nav>
  <slot />
  </main>
  <footer class=" h-60 flex justify-center items-center bg-stone-950">
    <div class="flex text-white">
        <div class="flex justify-center border-b-1 border-white">
        <button class=" text-7xl" on:click={scrollToTop}>^</button>
        </div>
    </div>
  </footer>


