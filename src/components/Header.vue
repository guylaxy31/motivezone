<template>
  <div class="header-container">
    <div class="header-bg">
      <div class="nav-container">
        <div class="motive-logo">
          <img src="@/assets/logo/motive-logo.svg" alt="motive logo" />
        </div>
        <div class="menu-list">
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Our Work</a></li>
            <li><a href="#">About US</a></li>
            <li><a href="#">Review</a></li>
            <li><a href="#">Contact US</a></li>
          </ul>
        </div>
        <div class="say-btn">
          <p>Say Hi</p>
        </div>
      </div>
      <div class="header-content">
        <div class="content-text">
          <h1>We Build Brands That Lead & Inspire</h1>
          <p>
            On the other hand, we denounce with righteous indignation and
            dislike men who are so beguiled and demoralized by the charms of
            pleasure of the moment, so blinded by desire, that they cannot
            foresee the pain and trouble
          </p>
          <div class="read-btn"><p>Read more</p></div>
        </div>
        <div class="content-group-img">
          <img src="@/assets/images/header-group.svg" alt="group image" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default { name: "Header" };
</script>

<style scpoed>
.header-container {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
}

.header-bg {
  min-width: 100%;
  background-image: url("../assets/images/header-bg.svg");
  min-height: 950px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}

.nav-container {
  margin-top: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 80%;
}
.menu-list {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

.menu-list ul {
  display: flex;
  flex-direction: row;
  gap: 40px;
  flex-wrap: wrap;
}
.menu-list ul li {
  list-style-type: none;
}

.menu-list ul li a {
  text-decoration: none;
  color: #fff;
}

.menu-list ul li a:hover {
  color: #ffae2d;
}

.say-btn {
  background-color: #ff9c00;
  border-radius: 5px;
  width: 104px;
  height: 48px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.say-btn:hover {
  cursor: pointer;
}

.say-btn > p {
  color: #fff;
}

.header-content {
  display: flex;
  flex-direction: row;
  margin-top: 96px;
  align-items: center;
  gap: 144px;
}
.header-content .content-text {
  width: 696px;
}

.content-text h1,
p {
  margin: 0;
  color: #fff;
}
.content-text h1 {
  font-size: 50px;
  margin-bottom: 32px;
}
.content-text > p {
  font-size: 15px;
  margin-bottom: 40px;
}

.read-btn {
  width: 136px;
  height: 48px;
  background-color: #ff9c00;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px;
}

.read-btn:hover {
  cursor: pointer;
}

.read-btn > p {
  color: #fff;
}

.content-group-img {
}
</style>