<template>
  <div id="interest">
    <div class="interest-content">
      <h1 data-aos="fade-left" data-aos-duration="1000">
        Interested To Work With Us?
      </h1>
      <p class="interest-p1">
        Because it is pleasure, but because those who do not know how to pursue
        pleasure rationally encounter consequences that are extremely painful.
        Nor again is there anyone who loves or pursues or desires to obtain pain
      </p>
      <p class="interest-p2">
        Of itself, because it is pain, but because occasionally circumstances
        occur in which toil and pain can procure him some great pleasure
      </p>
      <div class="input-container">
        <input type="email" placeholder="Enter your email address" />
        <div class="send-btn"><p>Send</p></div>
      </div>
    </div>
    <div class="interest-img">
      <img src="@/assets/images/interest.svg" alt="interest image" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Interest",
};
</script>

<style scoped>
#interest {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  min-height: 496px;
}

.interest-img {
  position: absolute;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
}
.interest-img > img {
  margin-left: 32px;
  max-width: 631px;
}
.interest-content {
  z-index: 1;
  max-width: 595px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  align-self: flex-end;
  flex-wrap: wrap;
  padding-right: 10%;
  padding-left: 10%;
}
.interest-content h1 {
  font-size: 40px;
}
.interest-p1 {
  color: #28384e;
  font-size: 15px;
  margin-bottom: 40px;
}
.interest-p2 {
  color: #28384e;
  font-size: 15px;
  margin-bottom: 72px;
}

.input-container {
  width: 541px;
  height: 60px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.input-container input {
  width: 100%;
  height: 100%;
  padding-left: 24px;
  padding-right: 104px;
  background-color: #faf9f7;
  border-color: #ede5d9;
  border-radius: 5px;
  display: flex;
  border-top-style: hidden;
  border-right-style: hidden;
  border-left-style: hidden;
  border: 1px solid #cccccc;
}
.send-btn {
  position: absolute;
  display: flex;
  background-color: #ff9c00;
  font-weight: bold;
  color: #fff;
  padding-left: 24px;
  padding-right: 24px;
  padding-top: 16px;
  padding-bottom: 16px;
  border-radius: 5px;
  margin-left: 448px;
}
.send-btn:hover {
  cursor: pointer;
}

@media only screen and (max-width: 1200px) {
  .interest-img {
    margin-top: 620px;
  }
  .interest-img > img {
    max-width: 408px;
    margin-left: 64px;
  }
  .input-container {
    opacity: 0.95;
  }
}

@media only screen and (max-width: 992px) {
  .interest-content {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .interest-content > h1 {
    font-size: 28px;
  }
  .interest-content > p {
    font-size: 14px;
  }
  .input-container {
    width: 445px;
    height: 60px;
  }
  .send-btn {
    margin-left: 352px;
  }
}

@media only screen and (max-width: 662px) {
  .input-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
  }
  .input-container > input {
    display: flex;
    padding-right: 32px;
    margin-right: 8px;
    margin-bottom: 16px;
  }
  .send-btn {
    display: flex;
    position: relative;
    margin-left: 0;
    padding-top: 16px;
    padding-bottom: 16px;
    padding-left: 24;
    padding-right: 24;
    font-size: 14px;
  }

  .interest-img {
    justify-content: center;
  }
  .interest-img > img {
    width: 216px;
    margin-left: 0;
  }
}
</style>