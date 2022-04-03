<template>
  <div>
    <div>
      <div class="custom__svg">
        <svg
          data-aos="fade-up"
          data-aos-duration="2000"
          data-name="Layer 1"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1200 120"
          preserveAspectRatio="none"
        >
          <path
            d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z"
            class="shape-fill"
          ></path>
        </svg>
      </div>
      <div class="header__front">
        <v-row class="justify-end widthmin">
          <div class="mt-6">
            <ul class="d-flex">
              <li class="header-items"><a href="#about">About</a></li>
              <li class="header-items"><a href="#services">Services</a></li>
              <li class="header-items"><a href="#portfolio">Portfolio</a></li>
              <li class="header-items"><a href="#contact">Contact</a></li>
            </ul>
          </div>
        </v-row>
        <v-row
          style="margin-top: 12vh !important; color: white"
          class="widthmin align-center"
        >
          <v-col cols="12" md="7">
            <h1 style="font-size: 3em">Hi, my name is Samuel.</h1>
            <p class="mt-5" style="font-size: 1.6em">
              I'm a freelance web developer <br />
              with a focus on front end <br />
              design and development.
            </p>
            <div class="d-flex mt-8">
              <a href="#portfolio"
                ><v-btn light class="text-none">My Work</v-btn></a
              >
              <a href="#contact"
                ><v-btn dark class="ml-4 text-none btn__custom"
                  >Let's Talk</v-btn
                ></a
              >
            </div>
          </v-col>
          <v-col
            cols="12"
            md="5"
            class="d-none d-md-block"
            data-aos="zoom-in"
            data-aos-duration="3000"
            data-aos-delay="300"
          >
            <div class="main">
              <div>
                <img style="width: 40px; height: 40px" src="/vue.png" />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: 0s; width: 40px; height: 35px"
                  src="/boot.png"
                />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: -1s; width: 80px; height: 45px"
                  src="/js.png"
                />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: -2s; width: 40px; height: 35px"
                  src="/nuxt.png"
                />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: -3s; width: 40px; height: 40px"
                  src="/vuetify-logo.png"
                />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: -4s; width: 50px; height: 40px"
                  src="/sass.png"
                />
              </div>
              <div>
                <img
                  class="item"
                  style="animation-delay: -5s; width: 40px; height: 40px"
                  src="/css.png"
                />
              </div>

              <div>
                <img
                  class="item"
                  style="animation-delay: -6s; width: 40px; height: 40px"
                  src="/html5.png"
                />
              </div>
            </div>
          </v-col>
        </v-row>
      </div>
    </div>
    <v-container
      id="about"
      style="min-height: 100vh; background-color: #fcfcfc"
      fluid
    >
      <div class="widthmin mt-10">
        <h1
          style="text-align: center"
          data-aos="fade-down"
          data-aos-duration="1200"
        >
          About Me
        </h1>
        <v-row sty class="mt-8 align-center">
          <v-col
            data-aos="fade-right"
            data-aos-duration="1200"
            cols="12"
            md="5"
            class="part"
          >
            <img src="/profile.jpeg" alt="" />
          </v-col>
          <v-col cols="12" md="7" class="text-justify">
            <div
              style="background-color: white; border-radius: 10px;color;#575757"
              class="pa-6"
            >
              <p>
                I'm a software engineer specializing in web development using
                the MEVN stack. I have previously worked at a local startup
                which allowed me to get familiar with most stages of the
                software development process and learned to communicate well
                with clients and other team members. I've also done long-term
                contract work for clients using different web technologies.
              </p>
              <p>
                I graduated from Addis Ababa Science and Technology University,
                during which I learned about software architecture, design
                patterns, writing proper documentation, and many more
                industry-related topics.
              </p>
              <h2>Skills</h2>
              <div class="d-inline-block mt-2" style="margin-left: -10px">
                <v-chip
                  data-aos="zoom-in"
                  data-aos-duration="1000"
                  style="min-width: 100px; height: 40px"
                  class="mt-4 ml-3"
                  v-for="chip in chips"
                  :key="chip.name"
                  ><span
                    ><img
                      class="pa-1 pt-2"
                      :src="chip.image"
                      height="40px" /></span
                  >{{ chip.name }}</v-chip
                >
              </div>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-container>
    <v-container
      id="services"
      style="min-height: 100vh; background-color: #fff5eb"
      fluid
    >
      <div class="widthmin mt-10">
        <h1
          data-aos="fade-right"
          data-aos-duration="1000"
          style="text-align: center"
        >
          What I Do
        </h1>
        <v-row class="justify-space-between mt-16 widthmin">
          <v-col v-for="how in howItWorks" :key="how.header" cols="12" md="3">
            <div
              data-aos="fade-down"
              :data-aos-duration="how.duration"
              class="ml-2"
            >
              <img :src="how.image" style="width: 52px; height: 62px" alt="" />
              <h2 class="mt-2" style="color: #212331">
                <span
                  style="color: #fea74c; margin-left: -40px; margin-right: 10px"
                  >{{ how.headerNo }}</span
                >{{ how.header }}
              </h2>
              <p style="color: #212331" class="mt-2">{{ how.text }}</p>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-container>
    <v-container
      id="portfolio"
      style="min-height: 100vh; background-color: #fcfcfc"
      fluid
    >
      <div class="widthmin mt-16 pb-10">
        <h1
          data-aos="fade-down"
          data-aos-duration="1200"
          style="text-align: center"
        >
          Portfolio
        </h1>
        <v-row class="justify-start mt-5">
          <v-col
            v-for="port in portfolio"
            :key="port.title"
            cols="12"
            md="4"
            sm="6"
            class="mt-10"
          >
            <div style="width: 85%; margin: auto">
              <v-card
                style="
                  border-top-left-radius: 320px;
                  border-top-right-radius: 320px;
                  height: 360px;
                "
              >
                <div data-aos="flip-up" data-aos-duration="1400">
                  <v-img
                    class="portfolio__img"
                    style="
                      border-radius: 20px;
                      box-shadow: 0px 0px 4px 2px #ddd;
                    "
                    height="180"
                    :src="port.img"
                  ></v-img>
                </div>
                <v-card-title class="mt-2">{{ port.title }}</v-card-title>
                <v-card-text>
                  {{ port.description }}
                </v-card-text>
                <v-card-actions v-if="port.link != ''" class="ml-2">
                  <a target="_blank" :href="port.link"
                    ><v-icon class="linkstyle">mdi-link</v-icon></a
                  >
                </v-card-actions>
              </v-card>
            </div>
          </v-col>
        </v-row>
      </div></v-container
    >

    <v-container id="contact" fluid class="header__back mt-16">
      <div class="custom-shape-divider-top-1648914438">
        <svg
          data-name="Layer 1"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1200 120"
          preserveAspectRatio="none"
        >
          <path
            d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
            class="shape-fill"
          ></path>
        </svg>
      </div>
      <div class="widthmin">
        <h1 data-aos="fade-down"
          data-aos-duration="1200" style="text-align: center" class="mt-10">Get in touch</h1>
        <v-row class="mt-10" justify="center" data-aos="zoom-in"
          data-aos-duration="1200">
          <div>
            <v-btn style="width: 280px; padding: 25px" class="mt-4"
              ><v-icon style="color: #2b2d3d" class="mr-3">mdi-phone</v-icon
              >+251966925486</v-btn
            >
          </div>
          <div style="width: 100px"></div>
          <div>
            <a href="mailto:samuellegese98@gmail.com"
              ><v-btn style="width: 280px; padding: 25px" class="text-none mt-4"
                ><v-icon style="color: #2b2d3d" class="mr-3">mdi-email</v-icon
                >samuellegese98@gmail.com</v-btn
              ></a
            >
          </div>
        </v-row>
        <v-row class="mt-16" justify="center">
          <a target="_blank" href="https://github.com/sammy-prog"><img class="contacts" src="/git.png" alt="" /></a>
          <a target="_blank" href="https://www.linkedin.com/samuel-legese"><img class="contacts ml-3" src="/linked1.png" alt="" /></a>
          <a target="_blank" href="https://www.instagram.com/sammy_prog/"><img class="contacts ml-3" src="/instaimg.png" alt="" /></a>
          <a target="_blank" href="https://t.me/SteepDose"><img class="contacts ml-3" src="/tele5.png" alt="" /></a>
        </v-row>
      </div>
    </v-container>
  </div>
</template>

<script>
import aosMixin from "~/mixins/aos";
export default {
  name: "IndexPage",
  mixins: [aosMixin],
  data() {
    return {
      portfolio: [
        {
          title: "OneStream",
          description:
            "Alternative deisgn for the popular multi-streaming platform.",
          link: "https://onestream-sam.netlify.app/",
          img: "/portfolio/screenshot (2).png",
        },
        {
          title: "DiscoverOut",
          description:
            "landing page UI Built using the Sass framework and deployed on netlify.",
          link: "https://discoverout.netlify.app/",
          img: "/portfolio/screenshot (13).png",
        },
        {
          title: "OneDash",
          description: "Admin dashboard UI built using Vue and Vuetify.",
          link: "https://onedashboard.netlify.app/",
          img: "/portfolio/screenshot (10).png",
        },
        {
          title: "QruQru",
          description: "Digital art reviewer built using vue and Node.Js",
          link: "",
          img: "/portfolio/Screenshot (103).png",
        },
        {
          title: "Ninjable",
          description: "Web App that intends to gamify the entire HR process.",
          link: "",
          img: "/portfolio/ninjableportal.png",
        },
        {
          title: "PDS",
          description:
            "paultry diagnostics system is an electron app designed to provide faster diagnosis of paultry diseases.",
          link: "",
          img: "/portfolio/1.png",
        },
        // {
        //   title: "Ninjable/Admin",
        //   description:
        //     "Admin for Web App that intends to gamify the entire HR process.",
        //   link: "",
        //   img: "/portfolio/Integrations.png",
        // },
      ],
      howItWorks: [
        {
          image: "/figma.png",
          header: "Convert Mockups",
          headerNo: "01",
          text: "Convert UI mockups from sources like Figma and Adobe xd to working pages using various tech stacks.",
          duration: "1200",
        },
        {
          image: "/vue.png",
          header: "Build Web Apps",
          headerNo: "02",
          text: "Develop fullly functional websites using the Vue.Js ecosystem, along with Node.js, Express and Mongodb.",
          duration: "1700",
        },
        {
          image: "/graph.png",
          header: "API Development",
          headerNo: "03",
          text: "Implement common APIs based on architecture guidelines and frameworks using graphql or RESTFUL services.",
          duration: "2400",
        },
      ],
      chips: [
        {
          name: "HTML5",
          image: "/html5.png",
        },
        {
          name: "CSS3",
          image: "/css.png",
        },
        {
          name: "JavaScript",
          image: "/js.png",
        },
        {
          name: "Vue.Js",
          image: "/vue.png",
        },
        {
          name: "Vuetify.Js",
          image: "/vuetify-logo.png",
        },
        {
          name: "Nuxt.Js",
          image: "/nuxt.png",
        },
        {
          name: "BootStrap",
          image: "/boot.png",
        },
        {
          name: "Sass",
          image: "/sass.png",
        },
        {
          name: "Node.Js",
          image: "/node.webp",
        },
        {
          name: "Hasura",
          image: "/hasura.webp",
        },
        {
          name: "Electron",
          image: "/electron.png",
        },
        {
          name: "Rest",
          image: "/rest.webp",
        },
        {
          name: "GraphQL",
          image: "/graph.png",
        },
        {
          name: "Docker",
          image: "/Moby-logo.webp",
        },
        {
          name: "MongoDB",
          image: "/mongo.webp",
        },
        {
          name: "MySql",
          image: "/mysql.png",
        },
      ],
    };
  },
};
</script>

<style>
html {
  scroll-behavior: smooth;
}
* {
  font-family: "Quicksand", sans-serif;
}
body {
  overflow-x: hidden;
}
.widthmin {
  max-width: 90% !important;
  margin: auto !important;
}
.header-items {
  text-decoration: none;
  list-style: none;
  padding: 5px;
  line-height: 22.5px;
  margin-left: 2.5vw;
  margin-top: 5px;
}
.header-items a {
  text-decoration: none !important;
  color: #ffffff !important;
  font-weight: 600;
  font-size: 1.2em;
}
a {
  text-decoration: none !important;
}
.custom__svg {
  position: absolute;
  top: 85vh;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}

.custom__svg svg {
  position: relative;
  display: block;
  width: calc(127% + 1.3px);
  height: 150px;
}

.custom__svg .shape-fill {
  fill: #fcfcfc;
}
.header__front {
  background: linear-gradient(146deg, #2b2d3d 13%, #000000 93%) !important;
  height: 100vh;
}
.main {
  height: 48vh;
  width: 40vw;
  background-color: transparent;
  border-color: #eee;
  border-radius: 10px;
  border-width: 2px;
  display: grid;
  justify-content: center;
  align-content: center;
}
.main > * {
  grid-column: 1;
  grid-row: 1;
}
.item {
  animation: spinAround 7s linear infinite;
}
@keyframes spinAround {
  from {
    transform: rotate(0deg) translate(180px);
  }
  to {
    transform: rotate(360deg) translate(180px);
  }
}
.btn__custom {
  background: linear-gradient(
    90deg,
    rgb(134, 135, 136) 13%,
    rgb(83, 83, 83) 93%
  ) !important;
}

.part img {
  clip-path: polygon(0 75%, 0 0, 100% 0, 100% 75%, 50% 100%);
  border-radius: 20px;
  width: 410px;
  height: 420px;
}
.portfolio__img {
  transform: scale(1.01) rotate(-4.5deg);
  transform-origin: 65% 75%;
  transition: transform 1s, filter 0.1s ease;
}
.portfolio__img:hover {
  transform: scale(1) rotate(0deg);
}
.header__back {
  position: relative;
  color: white;
  background: linear-gradient(146deg, #2b2d3d 13%, #000000 93%) !important;
  min-height: 50vh;
}
.custom-shape-divider-top-1648914438 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}

.custom-shape-divider-top-1648914438 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 120px;
}

.custom-shape-divider-top-1648914438 .shape-fill {
  fill: #ffffff;
}
.linkstyle:hover {
  color: #2b2d3d;
}
.contacts {
  border-radius: 50%;
  border: 1px solid white;
  padding: 10px;
  height: 50px;
  width: 50px;
}
@media only screen and (max-width: 700px) {
  .part img {
    width: 270px;
    height: 280px;
    margin-left: 10%;
  }
}
</style>
