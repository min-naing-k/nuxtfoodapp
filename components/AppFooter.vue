<template>
  <footer>
    Copyright&#x000A9; <span>{{ year }}</span>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>

<style lang="scss" scoped>
span {
  color: #fff;
}
</style>
