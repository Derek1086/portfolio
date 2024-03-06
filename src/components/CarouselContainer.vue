<template>
  <div class="carousel">
    <div class="arrow">
      <v-btn icon="fa-solid fa-angle-left" variant="flat" @click="prevSlide" />
    </div>
    <div class="slides">
      <div
        v-for="(slide, index) in slides"
        :key="index"
        :id="'slide' + (index + 1)"
        v-show="currentIndex === index"
      >
        <h3>{{ slide.title }}</h3>
        <div class="carousel-box">
          <div class="listitems">
            <div
              v-for="skill in slide.skills"
              :key="skill.name"
              class="childSkills"
            >
              <v-icon
                :style="{
                  'background-image': `url('${skill.icon}')`,
                  'background-size': 'contain',
                  height: '55px',
                  width: '55px',
                }"
              />
              <br />
              <span class="text-caption">{{ skill.name }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="arrow">
      <v-btn icon="fa-solid fa-angle-right" variant="flat" @click="nextSlide" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentIndex: 0,
      slides: [
        {
          title: "Frontend",
          skills: [
            { name: "HTML5", icon: "HTML5.png" },
            { name: "CSS", icon: "css.png" },
            { name: "JavaScript", icon: "JavaScript.png" },
            { name: "TypeScript", icon: "TypeScript.png" },
            { name: "Material UI", icon: "mui.png" },
            { name: "ReactJS", icon: "Reactjs.png" },
            { name: "NextJS", icon: "Nextjs.png" },
            { name: "VueJS", icon: "vue.png" },
          ],
        },
        {
          title: "Backend",
          skills: [
            { name: "mongoDB", icon: "mongodb.png" },
            { name: "NodeJS", icon: "nodejs.png" },
            { name: "Firebase", icon: "Firebase.png" },
            { name: "Vercel", icon: "Vercel.png" },
          ],
        },
        {
          title: "Misc.",
          skills: [
            { name: "Python", icon: "Python.png" },
            { name: "Java", icon: "Java.png" },
            { name: "C++", icon: "cplusplus.png" },
            { name: "Lua", icon: "Lua.png" },
            { name: "Roblox Studio", icon: "RBX.png" },
          ],
        },
      ],
    };
  },
  methods: {
    nextSlide() {
      this.currentIndex = (this.currentIndex + 1) % this.slides.length;
    },
    prevSlide() {
      this.currentIndex =
        (this.currentIndex - 1 + this.slides.length) % this.slides.length;
    },
  },
};
</script>

<style scoped>
.carousel {
  width: 100%;
  text-align: center;
  display: flex;
}

.slides {
  width: 95%;
  height: 100%;
}

.arrow {
  width: 5%;
  height: 100%;
  margin-top: 5%;
}

.listitems {
  margin-top: 20px;
  display: flex;
  gap: 5%;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

.childSkills {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 100%;
}
</style>
