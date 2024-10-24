<template>
  <div>
    <page-header></page-header>
    <RouterView></RouterView>
  </div>

</template>

<style>
* {
  margin: 0%;
}
</style>

<script>

import PageHeader from "@/components/PageHeader.vue"
import { RouterView } from "vue-router";

export default {
  data() {

  },
  components: {
    PageHeader
  }
}

</script>