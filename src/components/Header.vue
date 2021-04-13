<template>
  <div class="header-container">
    <div class="header-bg">
      <div class="nav-container">
        <div class="drawer-btn">
          <img
            v-on:click="drawerhandler"
            src="@/assets/icons/drawer-menu.svg"
            alt="drawer icon"
          />
        </div>
        <div class="motive-logo">
          <img src="@/assets/logo/motive-logo.svg" alt="motive logo" />
        </div>
        <div
          v-bind:style="[this.drawerstate === false ? null : 'display:flex']"
          class="menu-list"
        >
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
export default {
  name: "Header",
  data() {
    return {
      drawerstate: false,
    };
  },
  computed: {},
  methods: {
    drawerhandler() {
      this.drawerstate = !this.drawerstate;
    },
  },
};
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
  border-radius: 4px;
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
  width: 100%;
  flex-direction: row;
  margin-top: 232px;
  justify-content: flex-start;
  align-items: center;
}
.content-text {
  z-index: 1;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  max-width: 696px;
  margin-left: 10%;
  margin-right: 10%;
}

.content-group-img {
  position: absolute;
  display: flex;
  width: 95%;

  justify-content: flex-end;
}

.content-group-img > img {
  width: 560px;
}
.drawer-btn {
  position: absolute;
  width: 100%;
  display: none;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  margin-top: 16px;
  margin-right: 32px;
}

.drawer-btn > img {
  width: 24px;
}

.drawer-btn > img:hover {
  cursor: pointer;
}

.content-text h1,
p {
  margin: 0;
  color: #fff;
}
.content-text h1 {
  font-size: 48px;
  margin-bottom: 32px;
  line-height: 72px;
}
.content-text > p {
  font-size: 15px;
  margin-bottom: 40px;
  line-height: 24px;
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

.read-btn:hover {
  cursor: pointer;
}

.read-btn > p {
  color: #fff;
}

@media only screen and (max-width: 1200px) {
  .nav-container {
    justify-content: flex-end;
  }
  .header-content {
    margin-top: 104px;
  }
  .menu-list {
    width: 70%;
  }
  .motive-logo {
    width: 30%;
  }
  .say-btn {
    margin-top: 16px;
  }

  .content-text {
    max-width: 568px;
  }
  .content-group-img > img {
    width: 282px;
  }
}

@media only screen and (max-width: 992px) {
  .nav-container {
    justify-content: center;
  }
  .motive-logo {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-bottom: 16px;
  }

  .menu-list {
    width: 100%;
    display: flex;
    justify-content: center;
  }
  .content-text {
    max-width: 472px;
    z-index: 1;
  }
  .content-text > h1 {
    font-size: 40px;
    margin-bottom: 24px;
    line-height: 40px;
  }

  .content-group-img > img {
    margin-bottom: -328px;
  }
}

@media only screen and (max-width: 662px) {
  .menu-list {
    display: none;
  }
  .menu-list ul {
    display: flex;
    width: 100%;
    padding: 0;
    flex-direction: column;
    gap: 0;
    align-items: center;
  }
  .menu-list ul li {
    width: 100%;
    display: flex;
    justify-content: center;
    padding-top: 8px;
    padding-bottom: 8px;
  }

  .drawer-btn {
    display: flex;
    margin-top: 8px;
  }
  .content-group-img {
    justify-content: center;
    margin-bottom: -120px;
    width: 100%;
    margin-bottom: -584px;
  }
  .content-group-img > img {
    width: 218px;
    margin-bottom: 0;
  }

  .content-text > h1 {
    font-size: 24px;
  }

  .content-text > p {
    font-size: 14px;
  }
  .say-btn {
    margin-top: 0;
    width: 72px;
    height: 40px;
  }
  .say-btn > p {
    font-size: 14px;
  }
  .read-btn {
    width: 88px;
    height: 40px;
    align-self: center;
  }
  .read-btn > p {
    font-size: 14px;
  }

  .motive-logo > img {
    width: 192px;
  }
}
</style>

 