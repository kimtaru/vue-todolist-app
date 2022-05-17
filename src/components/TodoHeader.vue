<template>
  <header>
    <h1>{{ this.getTitle }}</h1>
  </header>
</template>

<script>
import { mapState, mapGetters } from "vuex";

export default {
  computed: {
    ...mapGetters(["getTitle"])
  }
};
</script>
<!-- scoped : css style이 컴포넌트 안에서만 유효 -->
<style scoped>
h1 {
  color: #2f3b52;
  font-weight: 900;
  margin: 2.5rem 0 1.5rem;
}
</style>
