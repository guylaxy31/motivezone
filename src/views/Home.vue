<template>
  <div id="home">
    <Header />
    <Services />
    <Helpwith />
    <Interest />
    <Project />
    <Technician />
    <Company />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Services from "@/components/Services.vue";
import Helpwith from "@/components/Helpwith.vue";
import Interest from "@/components/Interest.vue";
import Project from "@/components/Project.vue";
import Company from "@/components/Company.vue";
import Technician from "@/components/Technician.vue";
export default {
  name: "Home",
  components: {
    Header,
    Services,
    Helpwith,
    Interest,
    Project,
    Company,
    Technician,
  },
};
</script>

<style >
#home {
  display: flex;
  width: 100%;
  flex-direction: column;
}

@media only screen and (max-width: 1200px) {
  #interest {
    margin-bottom: 160px;
  }
}

@media only screen and (max-width: 661px) {
  #interest {
    margin-bottom: 64px;
  }
}
</style>
