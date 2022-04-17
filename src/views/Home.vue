<template>
  <v-layout column justify-center align-center class="mt-4 pt-2">
    <VueCompareImage
      class="hidden-md-and-down"
      hover
      :style="{ minWidth: '1300px' }"
      :sliderLineWidth="sliderLine"
      :handleSize="hSize"
      :leftImage="leftImage"
      :rightImage="rightImage"
      :sliderPositionPercentage="sliderPosition"
    />
    <VueCompareImage
      class="hidden-lg-and-up"
      hover
      :style="{ maxWidth: '400px' }"
      :sliderLineWidth="sliderLine"
      :handleSize="hSize"
      :leftImage="leftImage2"
      :rightImage="rightImage2"
      :sliderPositionPercentage="sliderPosition"
    />

    <br>

    <vue-typer class="headline" :repeat="0" text="Dee Pu Lak"></vue-typer>
    <vue-typer
      :text="text1"
      :repeat="Infinity"
      :shuffle="false"
      initial-action="erasing"
      :pre-type-delay="70"
      :type-delay="70"
      :pre-erase-delay="1980"
      :erase-delay="150"
      erase-style="select-back"
      :erase-on-complete="false"
      caret-animation="smooth"
    ></vue-typer>
    <br>
    <v-flex xs12 sm6 md4 lg4 xl4>
      <v-card flat color="transparent" max-width="500">
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">
              <span>About</span>
              <span class="blue--text">Me</span>
            </h3>
            <div>
              <p>
                Hello! I’m Deepu. I'm a full-stack web developer who
                is passionate about
                <span
                  class="green--text font-weight-bold"
                ></span> building great user experiences,
                fighting for simplicity over complexity and constantly learning.
                I'm also making responsive web apps, ios and android application.
              </p>
            </div>
          </div>
        </v-card-title>

        <v-card-actions class="hidden-sm-and-down">
          <v-btn
            v-for="icon in icons"
            :key="icon.icon"
            fab
            dark
            outline
            color="#FF3A3F"
            :href="icon.href"
            target="_blank"
          >
            <v-icon dark>{{icon.icon}}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-card-actions class="hidden-md-and-up justify-center">
          <v-btn
            v-for="icon in icons"
            :key="icon.icon"
            small
            fab
            dark
            outline
            color="#FF3A3F"
            :href="icon.href"
            target="_blank"
          >
            <v-icon dark>{{icon.icon}}</v-icon>
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import { VueTyper } from "vue-typer";
import VueCompareImage from "vue-compare-image";

export default {
  metaInfo: {
    title: "Home",
    titleTemplate: "%s ← Dee's Space",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      { name: "description", content: "Dees's Portfolio" },
      { charset: "utf-8" },
      { property: "og:title", content: "Dee's Space" },
      { property: "og:site_name", content: "Dee's Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://dees.space" },
      {
        property: "og:image",
        //content: "https://i.imgur.com/Dcz2PGx.jpg"
        content: "https://cdn.pixabay.com/photo/2018/06/08/00/48/developer-3461405__340.png"
      },
      { property: "og:description", content: "Dee's Portfolio" }
    ]
  },
  components: {
    "vue-typer": VueTyper,
    VueCompareImage
  },
  data() {
    return {
      icons: [
        {
          href: "https://www.facebook.com/dipu.pulock/",
          icon: "fab fa-facebook-f"
        },
       { href: "https://www.instagram.com/its__elliott__/", icon: "fab fa-instagram" },
       {
          href: "https://www.youtube.com/channel/UCbRH_m9qoOxYggiUUgx-j1w",
          icon: "fab fa-youtube"
        },
        {
          href: "https://www.linkedin.com/in/deepu-pulaak-b84b73175/",
          icon: "fab fa-linkedin-in"
        },
        
         { href: "", icon: "fab fa-twitter" },
        {
          href: "",
          icon: "fas fa-envelope"
        },
        
      ],
      text1: ["Full-Stack Developer", "Web Developer", "Web Designer"],
      //leftImage: "https://i.imgur.com/bU50uS9.jpg",
      //leftImage: "https://i.pinimg.com/originals/95/cf/9d/95cf9d8936d115c734fedc06185437ab.jpg",
      //leftImage: "https://cdn.pixabay.com/photo/2021/08/04/13/06/software-developer-6521720__480.jpg",
      leftImage: "https://wallpaper.dog/large/20512774.png",
      //rightImage: "https://i.imgur.com/z3ZoEEw.jpg",
      //rightImage: "https://wallpaper.dog/large/20512774.png",
      rightImage: "https://cdn.pixabay.com/photo/2021/08/04/13/06/software-developer-6521720__480.jpg",
      //leftImage2: "https://i.imgur.com/SXBitjh.jpg",
      leftImage2: "https://wallpaper.dog/large/20512774.png",
      //rightImage2: "https://i.imgur.com/Dcz2PGx.jpg",
      //rightImage2: "https://i.pinimg.com/originals/95/cf/9d/95cf9d8936d115c734fedc06185437ab.jpg",
      rightImage2: "https://cdn.pixabay.com/photo/2018/06/08/00/48/developer-3461405__340.png",
      sliderLine: 0,
      hSize: 0,
      sliderPosition: 0.5
    };
  }
};
</script>
<style>
@keyframes rocking {
  0%,
  100% {
    transform: rotateZ(-10deg);
  }

  50% {
    transform: rotateZ(10deg);
  }
}

.vue-typer {
  font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
  font-size: 25px;
}
.vue-typer .custom.char.typed {
  color: #4a15f7;
}
.vue-typer .custom.char.selected {
  color: #b92401;
}

.vue-typer .custom.caret {
  animation: rocking 1s ease-in-out 0s infinite;
}
.vue-typer .custom.caret.typing {
  background-color: green;
}
.vue-typer .custom.caret.selecting {
  display: inline-block;
  background-color: #e91e63;
}
</style>

