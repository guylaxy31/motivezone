<template>
  <div id="home">
    <Header />
    <Services />
    <Helpwith />
    <Interest />
    <Project />
    <Technician />
    <Company />
    <Footer />
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
import Footer from "@/components/Footer.vue";
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "Home",
  created() {
    AOS.init();
  },
  components: {
    Header,
    Services,
    Helpwith,
    Interest,
    Project,
    Company,
    Technician,
    Footer,
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
