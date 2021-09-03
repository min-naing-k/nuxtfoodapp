<template>
  <main class="container">
    <AppHeader />
    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppRestaurantInfo from "../components/AppRestaurantInfo";
import AppHeader from "../components/AppHeader";
export default {
  components: {
    AppRestaurantInfo,
    AppHeader
  }
};
</script>
