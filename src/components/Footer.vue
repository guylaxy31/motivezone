<template>
  <div id="footer">
    <div class="footer-menu-list">
      <div class="footer-menu-col-main">
        <img src="@/assets/logo/uixzone-logo.svg" alt="uixzone logo" />
        <p>
          On the other hand, we denounce with righteous indignation and dislike
          men.
        </p>
        <p class="main-bold-text">Interested To Work With Us</p>
        <div class="input-field">
          <input type="email" placeholder="Enter your email address" />
          <div class="send-btn"><p>Send</p></div>
        </div>
      </div>
      <div class="footer-menu-col">
        <h3>Company</h3>
        <a href="#">About Us</a>
        <a href="#">Portfolio</a>
        <a href="#">Page</a>
        <a href="#">FAQ</a>
        <a href="#">Reviews</a>
      </div>
      <div class="footer-menu-col">
        <h3>Support</h3>
        <a href="#">Contact Us</a>
        <a href="#">Privacy policy</a>
        <a href="#">tram of use</a>
        <a href="#">Buy & Sell</a>
        <a href="#">Reviews</a>
      </div>
      <div class="footer-menu-col">
        <h3>Contact</h3>
        <a href="#">Madani Ave, usa 1212</a>
        <a href="#">+8802-55662000</a>
        <a href="#">Email: www.uixzone12.com</a>
        <a href="#">Buy & Sell</a>
        <a href="#">Reviews</a>
      </div>
    </div>

    <hr />

    <div class="footer-contact">
      <div class="footer-policy">
        <a href="#">Terms of Service</a>
        <a href="#">Privacy Policy</a>
        <a href="#">Security</a>
      </div>
      <div class="footer-social">
        <img src="@/assets/logo/facebook.svg" alt="facebook logo" />
        <img src="@/assets/logo/twitter.svg" alt="twitter logo" />
        <img src="@/assets/logo/youtube.svg" alt="youtube logo" />
      </div>
      <div class="footer-copyright">© 2020 MotiveZone All rights reserved.</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
#footer {
  width: 100%;
  display: flex;

  background-color: #011021;
  flex-direction: column;
  align-items: center;
}
.footer-menu-list {
  display: flex;
  flex-direction: row;
  width: 80%;
  justify-content: center;
  margin-bottom: 88px;
  padding-top: 88px;
  gap: 100px;
  flex-wrap: wrap;
}
.footer-menu-col-main {
  display: flex;
  flex-direction: column;

  max-width: 450px;
  flex-wrap: wrap;
}

.footer-menu-col-main > p {
  margin-bottom: 40px;
  max-width: 347px;
  line-height: 24px;
}
.footer-menu-col-main > img {
  width: 175px;
  margin-bottom: 24px;
}

.main-bold-text {
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 24px;
}
.footer-menu-col {
  display: flex;
  flex-direction: column;
}
.footer-menu-col > h3 {
  color: #fff;
  margin-bottom: 36px;
  font-size: 18px;
}
.footer-menu-col > a {
  text-decoration: none;
  color: #a9b2bc;
  margin-bottom: 24px;
  font-size: 14px;
  width: fit-content;
}
.input-field {
  display: flex;
  flex-direction: row;
  width: 427px;
  height: 60px;
  background-color: #fff;
  border-radius: 5px;
}
.input-field > input {
  width: 75%;
  border-top-style: hidden;
  border-right-style: hidden;
  border-left-style: hidden;
  border: none;
  padding-left: 8px;
  padding-right: 8px;
}
.input-field > input:focus {
  outline: none;
}

.input-field .send-btn {
  width: 25%;
  background-color: #1b498a;
  display: flex;
  align-items: center;
  justify-content: center;
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
}

.send-btn:hover {
  cursor: pointer;
}

.send-btn > p {
  font-weight: bold;
  font-size: 14px;
  color: #fff;
}

hr {
  width: 80%;
  height: 1px;
  margin-bottom: 50px;
  background-color: #fff;
  border-width: 0;
  opacity: 0.11;
}

.footer-contact {
  display: flex;
  flex-direction: row;
  width: 80%;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 40px;
  flex-wrap: wrap;
}
.footer-social {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 20px;
  padding-left: 8px;
  padding-right: 8px;
}
.footer-social > img {
  cursor: pointer;
}
.footer-policy {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 24px;
  padding-left: 8px;
  padding-right: 8px;
}
.footer-policy > a {
  text-decoration: none;
  color: #a9b2bc;
}
.footer-copyright {
  color: #a9b2bc;
  padding-left: 8px;
  padding-right: 8px;
}

@media only screen and (max-width: 992px) {
  .footer-policy,
  .footer-social,
  .footer-copyright {
    margin-bottom: 16px;
  }

  .footer-contact {
    justify-content: center;
  }
}

@media only screen and (max-width: 662px) {
  .input-field {
    width: 100%;
  }
  .footer-policy,
  .footer-social,
  .footer-copyright {
    margin-bottom: 24px;
  }

  .footer-policy > a {
    font-size: 14px;
  }

  .footer-copyright {
    font-size: 12px;
  }

  .footer-menu-list {
    gap: 80px;
  }
  .footer-menu-col {
    align-items: center;
  }
}
</style>