<template>
  <div id="project">
    <div class="pj-bg">
      <div class="pj-title">
        <h1>Our Latest Project</h1>
        <p>
          To take a trivial example, which of us ever undertakes laborious
          physical exercise, except to obtain some advantage But who has any
          right
        </p>
      </div>
      <div class="pj-card-list">
        <div class="pj-card">
          <img src="@/assets/images/project01.svg" alt="project image1" />
          <h1>Business & corporate</h1>
          <p>
            Find fault with a man who chooses to enjoy a pleasure that has no
            annoying.
          </p>
          <div class="learn-btn">
            <p>Learn More</p>
            <img src="@/assets/icons/arr-right-orange.svg" alt="arrow right" />
          </div>
        </div>
        <div class="pj-card">
          <img src="@/assets/images/project02.svg" alt="project image1" />
          <h1>Food & restaurant</h1>
          <p>
            Temporibus autem quibusdam et aut officiis debitis aut rerum
            necessitatibus.
          </p>
          <div class="learn-btn">
            <p>Learn More</p>
            <img src="@/assets/icons/arr-right-orange.svg" alt="arrow right" />
          </div>
        </div>
        <div class="pj-card">
          <img src="@/assets/images/project03.svg" alt="project image1" />
          <h1>Travel & tourism</h1>
          <p>
            Find fault with a man who chooses to enjoy a pleasure that has no
            annoying.
          </p>
          <div class="learn-btn">
            <p>Learn More</p>
            <img src="@/assets/icons/arr-right-orange.svg" alt="arrow right" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",
};
</script>

<style>
#project {
  width: 100%;
  display: flex;
  margin-top: 128px;
  margin-bottom: 120px;
}
.pj-bg {
  background-image: url("../assets/images/project-bg.svg");
  min-width: 100%;
  min-height: 1069px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: flex-start;
  padding-bottom: 72px
}

.pj-title {
  display: flex;
  flex-direction: column;
  padding-left: 10%;
  padding-right: 10%;
  align-items: center;
  margin-top: 96px;
  margin-bottom: 64px;
}

.pj-title > h1 {
  font-size: 40px;
  margin: 0;
  color: #fff;
  margin-bottom: 24px;
}
.pj-title > p {
  margin: 0;
}

.pj-card-list {
  display: flex;
  width: 100%;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
  gap: 32px;
}
.pj-card {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex-wrap: wrap;
  max-width: 460px;
}
.pj-card > img {
  margin-bottom: 24px;
}
.pj-card > h1 {
  color: #fff;
  font-size: 20px;
}
.pj-card > p {
  margin-bottom: 32px;
}

.learn-btn {
  display: flex;
  width: 104px;

  flex-direction: row;
}

.learn-btn > p {
  color: #ff9c00;
  margin-right: 8px;
}
.learn-btn:hover {
  cursor: pointer;
}

@media only screen and (max-width: 1200px) {
  .pj-card {
    max-width: 360px;
  }

  .pj-card > img {
    width: 360px;
  }
}
@media only screen and (max-width: 992px) {
  .pj-title h1 {
    font-size: 28px;
  }
}

@media only screen and (max-width: 768px) {
  .pj-card {
    max-width: 320px;
  }
  .pj-card > img {
    width: 320px;
  }
}

@media only screen and (max-width: 662px) {
  .pj-card {
    max-width: 240px;
  }
  .pj-card > img {
    width: 240px;
  }
  .pj-card > h1 {
    font-size: 18px;
  }
  .pj-card > p {
    font-size: 14;
  }
  .learn-btn > p {
    font-size: 14px;
  }
}
</style>