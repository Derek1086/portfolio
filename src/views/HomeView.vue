<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col
            cols="12"
            style="display: flex; justify-content: center; align-items: center"
          >
            <div style="position: relative; z-index: 1" class="mt-16">
              <h1 class="text-grey">Hello,</h1>
              <h1 class="text-white">I'm Derek Avila</h1>
              <span class="text-grey"
                >Aspiring Web Developer and Software Engineer</span
              >
              <br />
              <v-btn tile dark class="mt-4 download-btn" @click="downloadPDF">
                Download Resume
              </v-btn>
              <div>
                <v-btn
                  class="m1-10"
                  icon="fa-brands fa-github"
                  variant="plain"
                  color="#ffffff"
                  @click="openLink('https://github.com/Derek1086')"
                />
                <v-btn
                  class="m1-10"
                  icon="fa-brands fa-linkedin-in"
                  variant="plain"
                  color="#ffffff"
                  @click="
                    openLink(
                      'https://www.linkedin.com/in/derek-avila-950657236/'
                    )
                  "
                />
              </div>
            </div>
          </v-col>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            ></div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" id="about">
        <div class="pre-extra">
          <span class="text-grey">Get To Know More</span>
          <h1 class="text-black">About Me</h1>
          <br />
          <div style="display: flex; gap: 10%">
            <v-card class="item-card" elevation="2" style="width: 45%">
              <v-icon class="fa-solid fa-graduation-cap" />
              <h3 class="mt-4">Education</h3>
              <span class="text-grey">Texas State University</span><br />
              <span class="text-grey"
                >Bachelor's of Science in Computer Science</span
              >
            </v-card>
            <v-card class="item-card" elevation="2" style="width: 45%">
              <v-icon class="fa-solid fa-award" />
              <h3 class="mt-4">Certifications</h3>
              <span class="text-grey">Udemy</span><br />
              <span class="text-grey"
                >React - The Complete Guide (incl Hooks, React Router,
                Redux)</span
              ></v-card
            >
          </div>
          <p class="text-grey mt-4">
            I'm a passionate software developer with a solid foundation in help
            desk support. Graduated from Texas State University in December 2023
            with a Bachelor of Science in Computer Science, I possess a robust
            understanding of core principles. My commitment to continuous
            learning drives me to stay updated on industry trends. I'm
            enthusiastic about leveraging my troubleshooting skills to craft
            innovative and user-friendly applications. Specializing in both
            front-end and back-end development, I excel in React.js. Its
            efficiency and versatility resonate with me, allowing me to
            seamlessly bridge the gap between user interface design and robust
            back-end functionality. My unique perspective from a help desk
            environment enhances my development work, ensuring solutions that
            exceed user expectations.
          </p>
        </div>
      </v-col>
      <br />
      <br />
      <br />
      <v-divider />
      <v-col cols="12" id="portfolio">
        <div class="pre">
          <br />
          <br />
          <br />
          <span class="text-grey">Browse My</span>
          <h1 class="text-black">Projects</h1>
          <br />
          <v-row>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="Sentiment_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Sentiment Analysis</v-card-title>
                <v-card-subtitle> October 2022 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  This Java program classifies a set of movie reviews as
                  positive or negative based on their sentiment. This project
                  was completed for my Object-Oriented Design and Programming
                  class.
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                  "
                >
                  <div style="width: 100%; margin-bottom: 20px">
                    <v-icon
                      style="
                        background-image: url('Java.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Java</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                  "
                >
                  <div style="width: 50%; margin-bottom: 20px">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink(
                          'https://github.com/Derek1086/Sentiment_Analysis/tree/main/Sentiment_Analysis'
                        )
                      "
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="Expense_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Budget Manager</v-card-title>

                <v-card-subtitle> December 2022 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  Budget Manager is an app built with React.js to help manage
                  your month-to-month expenses. Users can edit their monthly
                  budget and add/remove expenses. After adding an expense, it
                  will generate a pie chart so the user can visualize their
                  expenses.
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('Reactjs.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">ReactJS</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('css.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">CSS</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('JavaScript.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">JavaScript</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink('https://github.com/Derek1086/expense-app')
                      "
                    />
                  </div>
                  <div style="width: 50%">
                    <h4>Live Demo</h4>
                    <v-btn
                      icon="fa-solid fa-arrow-up-right-from-square"
                      variant="tile"
                      @click="openLink('https://react-practice-9e728.web.app/')"
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="Notes_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Notes App</v-card-title>
                <v-card-subtitle> July 2023 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  Notes app is an app built with typescript to help manage any
                  notes you need, functions the same way as the ios notes app on
                  your iphone. The app utilizes speech recognition, allowing the
                  user to use their voice to write and filter their notes
                  without having to type.
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('Reactjs.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">ReactJS</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('mui.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Material UI</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('TypeScript.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">TypeScript</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('Firebase.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Firebase</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink('https://github.com/Derek1086/notes-app')
                      "
                    />
                  </div>
                  <div style="width: 50%">
                    <h4>Live Demo</h4>
                    <v-btn
                      icon="fa-solid fa-arrow-up-right-from-square"
                      variant="tile"
                      @click="
                        openLink('https://dereks-notes-web-app.web.app/notes')
                      "
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="RecSys_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Yelp Recommender System</v-card-title>
                <v-card-subtitle> November 2023 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  Created for a final project for my Recommender Systems class,
                  this program provides better recommendations to users than
                  yelp would by utilizing the surprise machine learning library
                  to provide personalized recommendations based on time slots.
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('Python.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Python</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink(
                          'https://github.com/Derek1086/RecommenderSystemsProj/tree/main/RecSysProject'
                        )
                      "
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="Fly_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Fly.mov</v-card-title>
                <v-card-subtitle> January 2024 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  This is a pvp based game built with the Roblox Studio game
                  engine using Lua as the programming langauge. The combat and
                  mechanics are inspired by Homelander from the TV show "The
                  Boys."
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <v-icon
                      style="
                        background-image: url('RBX.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Roblox Studio</span>
                  </div>
                  <div style="width: 50%">
                    <v-icon
                      style="
                        background-image: url('Lua.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">Lua</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink(
                          'https://github.com/Derek1086/fly_mov/tree/main'
                        )
                      "
                    />
                  </div>
                  <div style="width: 50%">
                    <h4>Live Demo</h4>
                    <v-btn
                      icon="fa-solid fa-arrow-up-right-from-square"
                      variant="tile"
                      @click="
                        openLink(
                          'https://www.roblox.com/games/16144887451/fly-mov'
                        )
                      "
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card
                class="item-card"
                elevation="2"
                max-width="344"
                min-height="675"
              >
                <v-img
                  style="border-radius: 20px"
                  src="HF_Census_Img.png"
                  height="200px"
                  cover
                ></v-img>
                <v-card-title>Holdfast Melee Census</v-card-title>
                <v-card-subtitle> February 2024 </v-card-subtitle>
                <v-card-text style="min-height: 200px">
                  Holdfast Melee Census is a tool created for the Holdfast:
                  Nations at War community to facilitate the tracking and
                  analysis of player location data. It provides an easy-to-use
                  interface for users to view census information on an
                  interactive map.
                </v-card-text>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('Reactjs.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">ReactJS</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('mongodb.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">mongoDB</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('TypeScript.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">TypeScript</span>
                  </div>
                  <div style="width: 25%">
                    <v-icon
                      style="
                        background-image: url('JavaScript.png');
                        background-size: contain;
                        height: 35px;
                        width: 35px;
                      "
                    />
                    <br />
                    <span class="text-caption">JavaScript</span>
                  </div>
                </div>
                <div
                  style="
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-bottom: 20px;
                  "
                >
                  <div style="width: 50%">
                    <h4>Code</h4>
                    <v-btn
                      icon="fa-brands fa-github"
                      variant="tile"
                      @click="
                        openLink('https://github.com/Derek1086/holdfast-census')
                      "
                    />
                  </div>
                  <div style="width: 50%">
                    <h4>Live Demo</h4>
                    <v-btn
                      icon="fa-solid fa-arrow-up-right-from-square"
                      variant="tile"
                      @click="openLink('https://holdfast-census.vercel.app/')"
                    />
                  </div>
                </div>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <br />
      <br />
      <br />
      <v-divider />
      <v-col id="skills">
        <div class="pre">
          <br />
          <br />
          <br />
          <span class="text-grey">Explore My</span>
          <h1 class="text-black">Skills</h1>
          <v-row>
            <v-col cols="12">
              <div class="child">
                <CarouselContainer />
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <br />
      <br />
      <br />
      <v-divider />
      <v-col cols="12" sm="12" id="contact">
        <div class="pre">
          <br />
          <br />
          <br />
          <span class="text-grey">Get In Touch</span>
          <h1 class="text-black">Contact Me</h1>
          <br />
          <div style="display: flex; gap: 10%">
            <v-card class="item-card" elevation="2" style="width: 100%">
              <div
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                  flex-wrap: wrap;
                "
              >
                <div style="width: 33.33%">
                  <v-icon icon="fa-solid fa-phone" /><br /><br />
                  <span class="text-grey">+1 512-635-9513</span>
                </div>
                <div style="width: 33.34%">
                  <v-icon icon="fa-solid fa-location-dot" /><br /><br />
                  <span class="text-grey"
                    >1647 Post Rd San Marcos, TX 78666
                  </span>
                </div>
                <div style="width: 33.33%">
                  <v-icon icon="fa-solid fa-envelope" /><br /><br />
                  <span class="text-grey">derekavila1086@gmail.com</span>
                </div>
              </div></v-card
            >
          </div>
        </div>
      </v-col>
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from "vue";
import NavBar from "../components/NavBar.vue";
import CarouselContainer from "../components/CarouselContainer.vue";

export default defineComponent({
  name: "HomeView",
  setup() {
    return {
      items: [
        {
          img: "HF_Census_Img.png",
        },
        {
          img: "Notes_Img.png",
        },
        {
          img: "Expense_Img.png",
        },
        {
          img: "RecSys_Img.png",
        },
        {
          img: "Sentiment_Img.png",
        },
        {
          img: "Fly_Img.png",
        },
        {
          img: "JavaScript.png",
        },
        {
          img: "mongodb.png",
        },
        {
          img: "HTML5.png",
        },
        {
          img: "mui.png",
        },
        {
          img: "Nextjs.png",
        },
        {
          img: "nodejs.png",
        },
        {
          img: "Reactjs.png",
        },
        {
          img: "TypeScript.png",
        },
        {
          img: "css.png",
        },
        {
          img: "vue.png",
        },
        {
          img: "Python.png",
        },
        {
          img: "Lua.png",
        },
        {
          img: "Java.png",
        },
        {
          img: "cplusplus.png",
        },
        {
          img: "Firebase.png",
        },
        {
          img: "RBX.png",
        },
        {
          img: "Vercel.png",
        },
      ],
    };
  },
  methods: {
    openLink(url) {
      window.open(url, "_blank");
    },
    downloadPDF() {
      const link = document.createElement("a");
      link.href = "Derek_A_Resume.pdf";
      link.target = "_blank";
      link.download = "Derek_A_Resume.pdf";

      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
    },
  },
  components: {
    NavBar,
    CarouselContainer,
  },
});
</script>

<style scoped>
.v-container {
  padding: 16px 0;
  background-color: white;
}

.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 300px;
  width: 100%;
  color: white;
}

.head::before {
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}

.head::after {
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}

.download-btn {
  border-radius: 20px !important;
  border: 2px solid white;
  background-color: black;
  color: white;
  transition: color 0.5s, background-color 0.5s, border-color 0.5s;
}

.download-btn:hover {
  color: black;
  background-color: white;
  border-color: black;
}

.item-card {
  border-radius: 20px !important;
  border: 2px solid black;
  padding: 20px;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  width: 100%;
}

.pre {
  width: 100%;
  text-align: center;
  padding: 0 200px;
}

.pre-extra {
  width: 100%;
  text-align: center;
  padding: 0 200px;
  margin-top: 5%;
}
</style>
