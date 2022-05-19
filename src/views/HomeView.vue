<template>
  <div class="home">
    <Navbar/>
    <Sidebaar/>
    <Tabs/>
  </div>
</template>

<script>
import Navbar from '../components/Navbaar.vue'
import Sidebaar from '../components/Sidebaar.vue'
import Tabs from '../components/Tabs.vue'
export default {
  name: "HomeView",
  components: {
    Navbar,
    Sidebaar,
    Tabs
  },
};
</script>
