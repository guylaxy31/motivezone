<template>
  <div id="Helpwith">
    <div class="help-bg">
      <div class="help-content">
        <h1 data-aos="fade-right" data-aos-duration="1000">We Are Hear To Help You With</h1>
        <p class="help-p1">
          But I must explain to you how all this mistaken idea of denouncing
          pleasure and praising pain was born and I will give you a complete
          account of the system, and expound the actual teachings of the great
          explorer
        </p>
        <p class="help-p2">
          Of the truth, the master-builder of human happiness. No one rejects,
          dislikes, or avoids pleasure itself
        </p>

        <div class="read-btn"><p>Read more</p></div>
      </div>

      <div class="help-group">
        <img src="@/assets/images/help-group.svg" alt="help group image" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.help-bg {
  min-width: 100%;
  background-image: url("../assets/images/help-bg.svg");
  min-height: 570px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
}

.help-content {
  z-index: 1;
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  max-width: 595px;
  padding-left: 10%;
  padding-right: 10%;
}
.help-p1 {
  margin-bottom: 40px;
  color: #000;
}
.help-p2 {
  color: #000;
  margin-bottom: 88px;
}

.read-btn {
  width: 136px;
  height: 48px;
  background-color: #ff9c00;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4px;
}
.help-group {
  position: absolute;
  display: flex;
  width: 98%;
  justify-content: flex-end;
}

.read-btn:hover {
  cursor: pointer;
}

@media only screen and (max-width: 1200px) {
  .help-group > img {
    width: 496px;
  }
}

@media only screen and (max-width: 992px) {
  .help-group {
    margin-bottom: -320px;
  }
  .help-group > img {
    width: 432px;
  }
  .help-content > h1 {
    font-size: 28px;
  }
  .help-content > p {
    font-size: 14px;
  }
}

@media only screen and (max-width: 662px) {
  .help-group > img {
    width: 272px;
    margin-bottom: -96px;
  }
  .read-btn {
    opacity: 0.8;
    width: 120px;
    height: 40px;
  }
  .read-btn > p {
    font-size: 14px;
  }
}
</style>