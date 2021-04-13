<template>
  <div id="technician">
    <div class="tech-box">
      <img src="@/assets/images/tech-profile.svg" alt="technician profile" />
      <div class="tech-details">
        <p class="tech-name">Carla stevens</p>
        <p class="tech-posi">Technical Director at MotiveZone</p>
        <p class="tech-desc">
          “On the other hand, we denounce with righteous indignation and dislike
          men who are so beguiled and demoralized by the charms of pleasure of
          the moment, so blinded by desire, that they cannot foresee the pain
          and trouble that are bound to ensue; and equal blame belongs to those
          who fail in their duty through weakness of will, which is the same as
          saying.”
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Technician",
};
</script>

<style scoped>
#technician {
  display: flex;
  width: 100%;
  flex-direction: row;
  justify-content: center;
  margin-bottom: 120px;
}

.tech-box {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  padding-left: 10%;
  padding-right: 10%;
  gap: 32px;
  flex-direction: row;
}
.tech-box > img {
  width: 534px;
}

.tech-details {
  max-width: 636px;
  padding-top: 64px;
  flex-wrap: wrap;
}
.tech-details > p {
  color: #072753;
}

.tech-name {
  font-size: 20px;
  margin-bottom: 24px;
}
.tech-posi {
  margin-bottom: 40px;
}

.tech-desc {
  line-height: 32px;
}

@media only screen and (max-width: 1520px) {
  .tech-box {
    justify-content: center;
  }
}

@media only screen and (max-width: 1200px) {
  .tech-box > img {
    width: 350px;
  }
}

@media only screen and (max-width: 662px) {
  .tech-box > img {
    width: 200px;
  }
  .tech-details {
    padding-top: 32px;
  }
  .tech-name {
    font-size: 18px;
    margin-bottom: 8px;
  }
  .tech-posi {
    margin-bottom: 16px;
  }
  .tech-desc {
    font-size: 14px;
  }
}
</style>