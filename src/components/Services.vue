<template>
  <div data-aos="fade-up" data-aos-easing="ease-out" id="services">
    <div class="service-title">
      <h1>Our Services</h1>
      <p>
        That are bound to ensue; and equal blame belongs to those who fail in
        their duty through weakness of will, which is the same as saying through
      </p>
    </div>
    <div class="service-content">
      <div class="service-item">
        <img src="@/assets/icons/web-des.svg" alt="web design icon" />
        <p class="service-item-title">Web Design</p>
        <p class="service-item-desc">
          Shrinking from toil and pain. These cases are perfectly simple and
          easy to distinguish. In a free hour, when our power.
        </p>
        <div class="learn-more-btn">
          <a class="service-item-learn" href="#">Learn More</a
          ><img src="@/assets/icons/arr-right.svg" alt="arrow right" />
        </div>
      </div>
      <div class="service-item">
        <img src="@/assets/icons/web-des.svg" alt="web design icon" />
        <p class="service-item-title">UI/UX Design</p>
        <p class="service-item-desc">
          When nothing prevents our being able to do what we like best, every
          pleasure is to be welcomed and every pain avoided.
        </p>
        <div class="learn-more-btn">
          <a class="service-item-learn" href="#">Learn More</a
          ><img src="@/assets/icons/arr-right.svg" alt="arrow right" />
        </div>
      </div>
      <div class="service-item">
        <img src="@/assets/icons/web-des.svg" alt="web design icon" />
        <p class="service-item-title">Graphic Design</p>
        <p class="service-item-desc">
          But in certain circumstances and owing to the claims of duty or the
          obligations of business it will frequently occur.
        </p>
        <div class="learn-more-btn">
          <a class="service-item-learn" href="#">Learn More</a
          ><img src="@/assets/icons/arr-right.svg" alt="arrow right" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped>
#services {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  flex-direction: column;

  align-items: center;
  padding-left: 10%;
  padding-right: 10%;
}

.service-title {
  display: flex;

  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  max-width: 734px;
}

.service-title > h1 {
  color: #072753;
  font-size: 40px;
  margin-bottom: 16px;
}

.service-title > p {
  color: #28384e;
  font-size: 15px;
  margin-bottom: 64px;
}

.service-content {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  width: 100%;
  justify-content: center;
  margin-bottom: 120px;
  gap: 96px;
}

.service-item {
  max-width: 332px;
}

.service-item-title {
  color: #072753;
  font-size: 24px;
  margin-bottom: 16px;
}

.service-item-desc {
  color: #28384e;
  margin-bottom: 54px;
  line-height: 24px;
}

.service-item > img {
  margin-bottom: 16px;
}

.service-item-learn {
  text-decoration: none;
  color: #1b498a;
  margin-right: 8px;
}

.learn-more-btn {
  width: fit-content;
}

.learn-more-btn:hover {
  cursor: pointer;
}

@media only screen and (max-width: 992px) {
  .service-item {
    display: flex;
    flex-direction: column;

    align-items: center;
  }
  .service-item > img {
    width: 128px;
    margin-bottom: 32px;
  }
  .service-title > h1 {
    font-size: 32px;
  }
  .service-item-title {
    font-size: 18px;
  }
  .service-item-desc {
    font-size: 14px;
  }
}
</style>



