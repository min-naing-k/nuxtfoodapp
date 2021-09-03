<template>
  <main class="container">
    <AppHeader />
    <AppRestaurantInfo :datasource="fooddata" />
  </main>
</template>

<script>
import AppRestaurantInfo from "../components/AppRestaurantInfo";
import AppHeader from "../components/AppHeader";
import { mapState } from "vuex";

export default {
  components: {
    AppRestaurantInfo,
    AppHeader
  },
  computed: {
    ...mapState(["fooddata"])
  }
};
</script>
