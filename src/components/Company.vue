<template>
  <div id="company">
    <div class="company-list">
      <img src="@/assets/logo/booking-logo.svg" alt="booking.com logo" />
      <img src="@/assets/logo/instacart-logo.svg" alt="instacard logo" />
      <img src="@/assets/logo/paypal-logo.svg" alt="paypal logo" />
      <img src="@/assets/logo/google-logo.svg" alt="google logo" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Company",
};
</script>

<style scoped>
#company {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  justify-content: center;
  margin-bottom: 120px;
}

.company-list {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 112px;
  width: 100%;
  justify-content: center;
  padding-left: 10%;
  padding-right: 10%;
}
.company-list > img {
  width: 215px;
}

@media only screen and (max-width: 992px) {
  .company-list {
    gap: 72px;
  }
  .company-list > img {
    width: 150px;
  }
}

@media only screen and (max-width: 662px) {
  .company-list > img {
    width: 120px;
  }
}
</style>