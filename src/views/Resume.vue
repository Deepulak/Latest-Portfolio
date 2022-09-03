<template>
  <v-layout row justify-center align-center wrap class="mt-4 pt-2">
    <v-flex xs12 sm12 md5 lg6 xl6 class="mt-4 pt-4">
      <h2 class="mb-4 pl-4 pt-2">Education</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">JAN 2019 -</div>
                <div class="caption font-weight-bold blue--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Full Stack Web Development Course</strong>
                <div class="caption mb-2">freeCodeCamp</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">JUN 2018 -</div>
                <div class="caption font-weight-bold blue--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Master of Arts</strong>
                <div class="caption mb-2">National Versity of Bangladesh</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">MAY 2017 -</div>
                <div class="caption font-weight-bold blue--text">SEP 2017</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Front-End Developer</strong>
                <div class="caption mb-2">Edureka</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">MAR 2016 -</div>
                <div class="caption font-weight-bold blue--text">APR 2017</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Higher Seconday Certificate</strong>
                <div class="caption mb-2">Dr Arifur Rahman Commerce College</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-flex xs12 sm12 md4 lg6 xl6 class="mt-4 pt-2">
      <h2 class="mb-4 pl-4">Experience</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">DEC 2016 -</div>
                <div class="caption font-weight-bold blue--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Freelance Frontend Developer</strong>
                <div class="caption mb-2">Remote</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="#3500D4" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">AUG 2019 -</div>
                <div class="caption font-weight-bold blue--text">APR 2021</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>IT Technician</strong>
                <div class="caption mb-2">MFS-EMMAUS</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Design</span>

          <span class="blue--text">Skills</span>
        </h2>
        <br>
        <strong>Photoshop</strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
        <strong>Adobe XD</strong>
        <v-progress-linear v-model="buffer2" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
        <strong>Zeplin</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
        <strong>Adobe Premiere Pro</strong>
        <v-progress-linear v-model="buffer4" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
        <strong>Figma</strong>
        <v-progress-linear v-model="buffer5" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
        <strong>Illustrator</strong>
        <v-progress-linear v-model="buffer6" :buffer-value="bufferValue" color="#DA0037" height="16"></v-progress-linear>
      </v-flex>
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Coding</span>
          <span class="blue--text">Skills</span>
        </h2>
        <br>
        <strong>VUE.js/strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>NEXT.js/strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>React.js/strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>Java/strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>HTML/CSS</strong>
        <v-progress-linear v-model="buffer2" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>Kotlin</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>Firebase</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>JavaScript</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>React Native</strong>
        <v-progress-linear v-model="buffer4" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>AWS</strong>
        <v-progress-linear v-model="buffer5" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>TypesScript</strong>
        <v-progress-linear v-model="buffer6" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>Python</strong>
        <v-progress-linear v-model="buffer7" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>C</strong>
        <v-progress-linear v-model="buffer8" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>C++</strong>
        <v-progress-linear v-model="buffer9" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>Django</strong>
        <v-progress-linear v-model="buffer10" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>MongoDB</strong>
        <v-progress-linear v-model="buffer11" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
        <strong>MySQL</strong>
        <v-progress-linear v-model="buffer12" :buffer-value="bufferValue" color="#4201FF" height="16"></v-progress-linear>
      </v-flex>
      <div class="mt-4 pt-2">
        <!-- <v-btn
          href="https://docs.google.com/document/d/1WSR42FEgUahJuR_RArW1wz7TfUBlgj13zekRidmQgs4/edit?usp=sharing"
          target="_blank"
          color="#ff3a3f"
          dark
          large
        >
          Download Resume
          <v-icon right dark>fas fa-file-download</v-icon>
        </v-btn>
        -->
        <v-btn
         target="_blank"
          color="#ff3a3f"
          dark
          large
        >
          Download Resume
          <v-icon right dark>fas fa-file-download</v-icon>
        </v-btn>
      </div>
    </v-layout>
  </v-layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Resume",
    titleTemplate: "%s ← Dee's Space",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        name: "description",
        content:
          "Vue NUXT HTML CSS JavaScript Design Adobe XD Photoshop Coding Skills Resume Work Web Developer Front-End"
      },
      { charset: "utf-8" },
      { property: "og:title", content: "Dee' Space" },
      { property: "og:site_name", content: "Dee' Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://Dee.space" },
      {
        property: "og:image",
        content: "https://i.imgur.com/Dcz2PGx.jpg"
      },
      {
        property: "og:description",
        content:
          "Vue NUXT HTML CSS JavaScript Design Adobe XD Photoshop Coding Skills Resume Work Web Developer Front-End"
      }
    ]
  },
  data() {
    return {
      value: 0,
      buffer1: 0,
      buffer2: 0,
      buffer3: 0,
      buffer4: 0,
      buffer5: 0,
      buffer6: 0,
      buffer7: 0,
      buffer8: 0,
      buffer9: 0,
      buffer10: 0,
      buffer11: 0,
      buffer12: 0,
      buffer13: 0,
      buffer14: 0,
      buffer15: 0,
      buffer16: 0,
      buffer17: 0,
      bufferValue: 100,
      interval: 0
    };
  },
  mounted() {
    this.startBuffer();
  },

  beforeDestroy() {
    clearInterval(this.interval);
  },

  methods: {
    startBuffer() {
      this.interval = setInterval(() => {
        this.buffer1 = 70;
        this.buffer2 = 60;
        this.buffer3 = 85;
        this.buffer4 = 70;
        this.buffer5 = 85;
        this.buffer6 = 65;
        this.buffer7 = 80;
        this.buffer8 = 80;
        this.buffer9 = 80;
        this.buffer10 = 90;
        this.buffer11 = 75;
        this.buffer12 = 80;
        this.buffer13 = 60;
        this.buffer14 = 60;
        this.buffer15 = 70;
        this.buffer16 = 80;
        this.buffer17 = 70;
      }, 800);
    }
  }
};
</script>
<style >
</style>

