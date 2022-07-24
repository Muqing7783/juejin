<template>
  <div id="app">
    <NavOne></NavOne>
    <NavTwo></NavTwo>
    <InfiniteScroll></InfiniteScroll>
  </div>
</template>

<script>

import NavOne from "@/components/NavOne";
import NavTwo from "@/components/NavTwo";
import InfiniteScroll from "@/components/InfiniteScroll";

export default {
  name: 'App',
  components: {
    NavOne,
    NavTwo,
    InfiniteScroll
  }
}
</script>

<style>

</style>
