<template>
  <div id="home">
    <Header />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "Home",
  components: {
    Header,
  },
};
</script>

<style >
#home {
  display: flex;
  width: 100%;
  flex-direction: column;
}
</style>
