<template>
  <div class="font-sans" id="nav">
    <nav class="flex items-center justify-between flex-wrap p-6">
      <div class="flex items-center flex-no-shrink text-black mr-6">
        <img src="../assets/logos/Y.png" class="w-2/12" />
        <span class="font-semibold text-xl tracking-tight">Yandry Villamo</span>
      </div>
      <div class="block sm:hidden">
        <button @click="toggle" class="flex items-center px-3 py-2 border rounded text-teal-lighter border-teal-light hover:text-white hover:border-white">
          <img class="h-3 w-3" src="https://img.icons8.com/ios/50/000000/menu--v1.png"/>
        </button>
      </div>
      <div :class="open ? 'block': 'hidden'"   class="w-full flex-grow sm:flex sm:items-center sm:w-auto"> 
        <div class="text-sm sm:flex-grow">
          <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-black mr-4">
            Docs
          </a>
          <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-black mr-4">
            Examples
          </a>
          <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-black">
            Blog
          </a>
        </div>
        <div>
          <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-black border-white hover:border-transparent hover:text-teal hover:bg-white mt-4 sm:mt-0">Download</a>
        </div>
      </div>

    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    msg: String,
  },
};




</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
