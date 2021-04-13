<template>
  <div id="home">
    <Header />
    <Services />
    <Helpwith />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Services from "@/components/Services.vue";
import Helpwith from "@/components/Helpwith.vue";
export default {
  name: "Home",
  components: {
    Header,
    Services,
    Helpwith,
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
