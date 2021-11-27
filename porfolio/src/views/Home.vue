<template>
  <div class="home">
    <navbar  id="nav"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";

export default {
  name: "Home",
  components: {
    Navbar,
  },
};

new Vue({
  el:'#nav',

   data: {
  	open: false,
  },
  methods: {
  	toggle() {
    	this.open = !this.open
    }
  }

})

</script>
