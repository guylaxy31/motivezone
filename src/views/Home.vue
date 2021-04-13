<template>
  <div id="home">
    <Header />
    <Services />
    <Helpwith />
    <Interest />
    <Project />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Services from "@/components/Services.vue";
import Helpwith from "@/components/Helpwith.vue";
import Interest from "@/components/Interest.vue";
import Project from "@/components/Project.vue";

export default {
  name: "Home",
  components: {
    Header,
    Services,
    Helpwith,
    Interest,
    Project,
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
