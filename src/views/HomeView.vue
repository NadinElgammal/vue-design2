<template>
  <div class="home">
    <Navbar/>
    <Sidebaar/>
    <Tabs/>
    <Chart/>
    <Statistics/>
    <Posts/>
  </div>
</template>

<script>
import Navbar from '../components/Navbaar.vue'
import Sidebaar from '../components/Sidebaar.vue'
import Tabs from '../components/Tabs.vue'
import Chart from '../components/Chart.vue'
import Statistics from '@/components/Statistics.vue'
import Posts from '../components/Posts/Posts.vue'

export default {
  name: "HomeView",
  components: {
    Navbar,
    Sidebaar,
    Tabs,
    Chart,
    Statistics,
    Posts
  },
};
</script>
