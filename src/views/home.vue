<template>
  <div class="home-container">
    <div data-role="Header" class="home-navbar-container">
      <div class="home-navbar">
        <img
          alt="image"
          src="https://cdn.discordapp.com/attachments/938769835763060766/945147220641067059/Ivans-Logo.png"
          class="home-image"
        />
        <div class="home-links-container">
          <span class="home-link navbar-Link">Contact</span>
        </div>
        <div data-type="BurgerMenu" class="home-burger-menu">
          <svg viewBox="0 0 1024 1024" class="home-icon">
            <path
              d="M128 256h768v86h-768v-86zM128 554v-84h768v84h-768zM128 768v-86h768v86h-768z"
            ></path>
          </svg>
        </div>
        <div data-type="MobileMenu" class="home-mobile-menu">
          <div class="home-container1">
            <span class="card-Heading home-heading">Logo</span>
            <div data-type="CloseMobileMenu" class="home-close-menu">
              <svg viewBox="0 0 1024 1024" class="home-icon2">
                <path
                  d="M810 274l-238 238 238 238-60 60-238-238-238 238-60-60 238-238-238-238 60-60 238 238 238-238z"
                ></path>
              </svg>
            </div>
          </div>
          <div class="home-links-container1">
            <span class="home-link1 navbar-Link">About</span>
            <span class="home-link2 navbar-Link">Experience</span>
            <span class="home-link3 navbar-Link">Portofolio</span>
            <span class="navbar-Link">Contact</span>
          </div>
        </div>
      </div>
    </div>
    <div class="home-section-separator"></div>
    <div class="home-section-separator1"></div>
    <div class="home-container2">
      <div class="home-hero">
        <div class="home-hero-text-container">
          <h1 class="home-heading1 section-Heading">Welcome</h1>
          <span class="home-text section-Text">
            <span>
              My name is Ivan Ryan. I am a programmer, community server manager
              and web designer
            </span>
            <span><span v-html="rawr8tj"></span></span>
          </span>
          <div class="home-cta-btn-container">
            <button class="home-cta-btn anchor button">
              <span class="home-text3">MY WORK</span>
            </button>
            <button class="home-cta-btn1 button anchor">ABOUT ME</button>
          </div>
        </div>
      </div>
    </div>
    <div class="home-features">
      <div class="home-heading-container">
        <h2 class="home-text4 section-Heading">Services</h2>
      </div>
      <div class="home-cards-container">
        <div class="home-card">
          <div class="home-icon-container">
            <img
              alt="image"
              src="/playground_assets/download%20%5B1%5D-200h.png"
              class="home-image1"
            />
          </div>
          <div class="home-content-container">
            <span class="home-heading2 card-Heading">Web Security</span>
            <span class="home-text5 card-Text">
              Detalied pentesting and privacy report for your website.
            </span>
          </div>
        </div>
        <div class="home-card1">
          <div class="home-icon-container1">
            <img
              alt="image"
              src="/playground_assets/download%20%5B2%5D1-200h.png"
              class="home-image2"
            />
          </div>
          <div class="home-content-container1">
            <span class="home-heading3 card-Heading">
              Community Server Hosting
            </span>
            <span class="home-text6 card-Text">
              I provide powerful dedicated servers that come with a custom
              pterodactyl panel for your community.
            </span>
          </div>
        </div>
      </div>
    </div>
    <div class="home-clients">
      <div class="home-heading-container1">
        <h1 class="home-text7 section-Heading">Clients</h1>
        <span class="home-text8 section-Text">
          Here we will put your clients&apos; or partners&apos; logos
        </span>
      </div>
      <div class="home-logo-container">
        <img
          alt="image"
          src="/playground_assets/default-img.svg"
          class="home-logo"
        />
        <img
          alt="image"
          src="/playground_assets/default-img.svg"
          class="home-logo1"
        />
        <img
          alt="image"
          src="/playground_assets/default-img.svg"
          class="home-logo2"
        />
        <img
          alt="image"
          src="/playground_assets/default-img.svg"
          class="home-logo3"
        />
        <img
          alt="image"
          src="/playground_assets/default-img.svg"
          class="home-logo4"
        />
      </div>
    </div>
    <div class="home-section-separator2"></div>
    <div class="home-footer-container">
      <div class="home-footer">
        <div class="home-container3">
          <div class="home-social-links"></div>
          <app-component></app-component>
        </div>
        <div class="home-copyright-container">
          <span class="home-link5 anchor">Copyright, 2022</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppComponent from '../components/component'

export default {
  name: 'Home',
  components: {
    AppComponent,
  },

  data() {
    return {
      rawr8tj: ' ',
    }
  },

  metaInfo: {
    title: "Ivan's Website",
    meta: [
      {
        property: 'og:title',
        content: "Ivan's Website",
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  height: auto;
  display: flex;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
}
.home-navbar-container {
  width: 100%;
  display: flex;
  z-index: 100;
  position: fixed;
  box-shadow: 5px 5px 10px 0px #d4d4d4;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  background-color: var(--dl-color-gray-white);
}
.home-navbar {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxcontent);
  align-items: center;
  padding-top: var(--dl-space-space-tripleunit);
  padding-left: var(--dl-space-space-tripleunit);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-tripleunit);
  justify-content: space-between;
  background-color: #000000;
}
.home-image {
  width: 150px;
  height: 93px;
  object-fit: cover;
}
.home-links-container {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
}
.home-link {
  color: #ffffff;
}
.home-burger-menu {
  display: none;
  align-items: flex-start;
  flex-direction: column;
}
.home-icon {
  width: 36px;
  height: 36px;
}
.home-mobile-menu {
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100vh;
  display: none;
  padding: var(--dl-space-space-tripleunit);
  position: absolute;
  align-items: flex-start;
  flex-direction: column;
  background-color: #fff;
}
.home-container1 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-doubleunit);
  flex-direction: row;
  justify-content: space-between;
}
.home-close-menu {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.home-icon2 {
  width: 24px;
  height: 24px;
}
.home-links-container1 {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.home-link1 {
  margin-bottom: var(--dl-space-space-unit);
}
.home-link2 {
  margin-bottom: var(--dl-space-space-unit);
}
.home-link3 {
  margin-bottom: var(--dl-space-space-unit);
}
.home-section-separator {
  width: 100%;
  height: 1px;
  display: flex;
  margin-top: var(--dl-space-space-tenunits);
  align-items: flex-start;
  flex-direction: column;
  background-color: var(--dl-color-gray-900);
}
.home-section-separator1 {
  width: 100%;
  height: 1px;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  background-color: #fffefe;
}
.home-container2 {
  width: 100%;
  height: 388px;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  background-color: #000000;
}
.home-hero {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxcontent);
  margin-top: var(--dl-space-space-fiveunits);
  align-items: center;
  padding-top: var(--dl-space-space-fiveunits);
  padding-left: var(--dl-space-space-tripleunit);
  margin-bottom: var(--dl-space-space-fiveunits);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-fiveunits);
  justify-content: space-between;
  background-color: #0e0e0e;
}
.home-hero-text-container {
  width: 1162px;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.home-heading1 {
  color: #ffffff;
  width: 1150px;
  height: 45px;
  margin-bottom: var(--dl-space-space-tripleunit);
}
.home-text {
  color: #ffffff;
  margin-bottom: var(--dl-space-space-fiveunits);
}
.home-cta-btn-container {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: flex-start;
}
.home-cta-btn {
  color: var(--dl-color-gray-white);
  text-align: center;
  padding-top: var(--dl-space-space-doubleunit);
  margin-right: var(--dl-space-space-fourunits);
  padding-left: var(--dl-space-space-tenunits);
  border-radius: var(--dl-radius-radius-radius8);
  padding-right: var(--dl-space-space-tenunits);
  padding-bottom: var(--dl-space-space-doubleunit);
  background-color: #c9c9c9;
}
.home-text3 {
  color: #101010;
}
.home-cta-btn1 {
  color: var(--dl-color-gray-black);
  text-align: center;
  padding-top: var(--dl-space-space-doubleunit);
  padding-left: var(--dl-space-space-tenunits);
  border-radius: var(--dl-radius-radius-radius8);
  padding-right: var(--dl-space-space-tenunits);
  padding-bottom: var(--dl-space-space-doubleunit);
  background-color: var(--dl-color-gray-white);
}
.home-features {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxcontent);
  margin-top: var(--dl-space-space-fiveunits);
  align-items: center;
  padding-top: var(--dl-space-space-fiveunits);
  padding-left: var(--dl-space-space-tripleunit);
  margin-bottom: var(--dl-space-space-fiveunits);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-fiveunits);
  background-color: #000000;
}
.home-heading-container {
  width: 45%;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-fiveunits);
  flex-direction: column;
}
.home-text4 {
  color: #ffffff;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-cards-container {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
}
.home-card {
  width: 542px;
  display: flex;
  align-items: center;
  padding-top: var(--dl-space-space-doubleunit);
  padding-left: var(--dl-space-space-doubleunit);
  margin-bottom: var(--dl-space-space-fourunits);
  padding-right: var(--dl-space-space-doubleunit);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-doubleunit);
}
.home-icon-container {
  width: 200px;
  display: flex;
  padding: var(--dl-space-space-unit);
  align-items: center;
  border-radius: var(--dl-radius-radius-round);
  margin-bottom: var(--dl-space-space-tripleunit);
  flex-direction: column;
}
.home-image1 {
  width: 100px;
  object-fit: cover;
}
.home-content-container {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.home-heading2 {
  color: #ffffff;
  margin-bottom: var(--dl-space-space-tripleunit);
}
.home-text5 {
  color: #ffffff;
  text-align: center;
}
.home-card1 {
  width: 600px;
  display: flex;
  align-items: center;
  padding-top: var(--dl-space-space-doubleunit);
  padding-left: var(--dl-space-space-doubleunit);
  margin-bottom: var(--dl-space-space-fourunits);
  padding-right: var(--dl-space-space-doubleunit);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-doubleunit);
}
.home-icon-container1 {
  width: 200px;
  display: flex;
  padding: var(--dl-space-space-unit);
  align-items: center;
  border-radius: var(--dl-radius-radius-round);
  margin-bottom: var(--dl-space-space-tripleunit);
  flex-direction: column;
  justify-content: center;
}
.home-image2 {
  width: 100px;
  object-fit: cover;
}
.home-content-container1 {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.home-heading3 {
  color: #ffffff;
  margin-bottom: var(--dl-space-space-tripleunit);
}
.home-text6 {
  color: #efe3e3;
  text-align: center;
}
.home-clients {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxcontent);
  align-items: center;
  padding-top: var(--dl-space-space-fiveunits);
  padding-left: var(--dl-space-space-tripleunit);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: column;
  padding-bottom: var(--dl-space-space-fiveunits);
  background-color: #000000;
}
.home-heading-container1 {
  width: 45%;
  display: flex;
  align-items: center;
  padding-left: var(--dl-space-space-tripleunit);
  margin-bottom: var(--dl-space-space-fiveunits);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: column;
}
.home-text7 {
  color: #ffffff;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-text8 {
  color: #ffffff;
  text-align: center;
}
.home-logo-container {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
}
.home-logo {
  width: 150px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-logo1 {
  width: 150px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-logo2 {
  width: 150px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-logo3 {
  width: 150px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-logo4 {
  width: 150px;
  object-fit: cover;
  margin-bottom: var(--dl-space-space-fourunits);
}
.home-section-separator2 {
  width: 100%;
  height: 1px;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  background-color: var(--dl-color-gray-900);
}
.home-footer-container {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  background-color: var(--dl-color-gray-white);
}
.home-footer {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxcontent);
  align-items: center;
  padding-top: var(--dl-space-space-tripleunit);
  padding-left: var(--dl-space-space-tripleunit);
  padding-right: var(--dl-space-space-tripleunit);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-tripleunit);
  justify-content: space-between;
  background-color: #000000;
}
.home-container3 {
  flex: 0 0 auto;
  width: auto;
  height: auto;
  display: flex;
  align-items: space-between;
  flex-direction: column;
}
.home-social-links {
  border: 2px dashed rgba(120, 120, 120, 0.4);
  display: flex;
  align-items: flex-start;
  flex-direction: row;
}
.home-copyright-container {
  display: flex;
  align-items: center;
  flex-direction: row;
}
.home-link5 {
  color: #ffffff;
}
@media(max-width: 991px) {
  .home-heading {
    text-align: center;
  }
  .home-hero {
    align-items: center;
    flex-direction: column;
    justify-content: center;
  }
  .home-hero-text-container {
    width: 80%;
    align-items: center;
    margin-bottom: var(--dl-space-space-fourunits);
  }
  .home-heading1 {
    text-align: center;
  }
  .home-text {
    text-align: center;
  }
  .home-text4 {
    text-align: center;
  }
}
@media(max-width: 767px) {
  .home-navbar {
    position: relative;
  }
  .home-links-container {
    display: none;
  }
  .home-burger-menu {
    display: flex;
    padding: var(--dl-space-space-halfunit);
    margin-left: var(--dl-space-space-tripleunit);
    border-radius: var(--dl-radius-radius-radius4);
    background-color: var(--dl-color-gray-black);
  }
  .home-icon {
    fill: var(--dl-color-gray-white);
  }
  .home-cta-btn {
    padding-left: var(--dl-space-space-fourunits);
    padding-right: var(--dl-space-space-fourunits);
  }
  .home-cta-btn1 {
    padding-left: var(--dl-space-space-fourunits);
    padding-right: var(--dl-space-space-fourunits);
  }
  .home-heading-container {
    width: 100%;
  }
  .home-cards-container {
    align-items: center;
    flex-direction: column;
  }
  .home-card {
    width: 70%;
    margin-bottom: var(--dl-space-space-tripleunit);
  }
  .home-card1 {
    width: 70%;
    margin-bottom: var(--dl-space-space-tripleunit);
  }
  .home-heading-container1 {
    width: 100%;
  }
}
@media(max-width: 479px) {
  .home-burger-menu {
    margin-left: var(--dl-space-space-doubleunit);
  }
  .home-hero-text-container {
    width: 100%;
  }
  .home-card {
    width: 100%;
  }
  .home-card1 {
    width: 100%;
  }
  .home-text7 {
    text-align: center;
  }
}
</style>
