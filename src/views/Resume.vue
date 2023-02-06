<template>
  <v-layout row justify-center align-center wrap class="mt-4 pt-2">
    <v-flex xs12 sm12 md5 lg6 xl6 class="mt-4 pt-4">
      <h2 class="mb-4 pl-4 pt-2">Education</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <!-- <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">JAN 2018 -</div>
                <div class="caption font-weight-bold green--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Full Stack Web Development Course</strong>
                <div class="caption mb-2">freeCodeCamp</div>
              </v-flex>
            </v-layout>
          </v-timeline-item> -->

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">Issued</div>
                <div class="caption font-weight-bold green--text">Feb 2020</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Microsoft Technology Associate: </strong>
                <div>Software Development Fundamentals (MTA)</div>
                <div class="caption mb-2">Microsoft
                  <v-btn
                    href="https://drive.google.com/file/d/10qH597x_EBfJjwcyVZUiQBQA3Mt3r_VD/view?usp=share_link"
                    target="_blank"
                    color="green"
                    dark
                    small
                  >
                    Certificate
                    <v-icon right dark>fas fa-file-download</v-icon>
                  </v-btn>
                </div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">JAN 2021 -</div>
                <div class="caption font-weight-bold green--text">AUGUST 2017</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Informatics Engineering</strong>
                <div class="caption">Universitas Advent Indonesia</div>
                <div class="caption mb-2">Bachelor's degree - 3.79</div>
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
          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">April 2022 -</div>
                <div class="caption font-weight-bold green--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Back End Developer</strong>
                <div class="caption mb-2">Blipcom · Remote Full-time - Jakarta Metropolitan Area</div>
                <p>Project Key Roles<br>
                - Develop mobile API with python - buid MRT API scheduler<br>
                - Develop clients website CMS ( Back-End )</p>
                <p>Technologies: Pytavia (Flask Framework), Ubuntu(Linux),<br>
                Python,Jinja template, MongoDB, Python Cherrypy,<br>
                HTML, JSON, ChartJS, Wordpress,CSS, AJAX, jQuery, <br>
                JavaScript, Apache, Github, Bootstrap, PHP, MySQL<br>
                Skills: Python (Programming Language)</p>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">APRIL 2021 -</div>
                <div class="caption font-weight-bold green--text">APRIL 2022</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Full Stack Developer</strong>
                <div class="caption mb-2">Barantum.com · Full-time - Jakarta Metropolitan Area</div>                             
                <p>Project Key Roles<br>
                - Develop CRM system <br>
                - Develop API ( Back-End ) using PHP/LUMEN<br>
                - Develop UX using vue framework, JS, HTML, CSS (Front-End) <br>
                - handle system flow (Frontend &amp; Backend)<br>
                - integrated system with outside api provider<br>
                - handle client requests<br>
                - Helping other stuff in application development<br>
                (Front-End or Back-End Programming, Guiding new developer)</p>

                <p>Technologies: Lumen (PHP framework), vue (frontend framwork), <br>
                Javascript, LDAP, Elastic Search, CSS, HTML, Bootstrap, MySQL,<br>
                Apache, PHP, Sendinblue, JSON, rest API</p>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">MAY 2020 -</div>
                <div class="caption font-weight-bold green--text">JULY 2020</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Web Developer</strong>
                <div class="caption mb-2">Universitas Advent Indonesia · Internship</div>
                <p>Project Key Roles<br>
                - Participate in Develop Registration System</p>

                <p>Technologies: Laravel (PHP framework),<br>
                Jquery, Javascript, CSS, HTML, Bootstrap, MySQL, Apache, PHP</p>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <!-- <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Design</span>

          <span class="green--text">Skills</span>
        </h2>
        <br>
        <strong>Photoshop</strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>Adobe XD</strong>
        <v-progress-linear v-model="buffer2" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>Zeplin</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
      </v-flex>
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Coding</span>
          <span class="green--text">Skills</span>
        </h2>
        <br>
        <strong>VUE/NUXT</strong>
        <v-progress-linear v-model="buffer4" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>HTML/CSS</strong>
        <v-progress-linear v-model="buffer5" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>JavaScript</strong>
        <v-progress-linear v-model="buffer6" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
      </v-flex> -->
      <div class="mt-4 pt-2">
        <v-btn
          href="https://drive.google.com/file/d/1qneDDIOLD-F1d9-bR34gdSeiljaaLym8/view?usp=sharing"
          target="_blank"
          color="green"
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
    titleTemplate: "%s ← Eldin's Space",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        name: "description",
        content:
          "Vue NUXT HTML CSS JavaScript Design Adobe XD Photoshop Coding Skills Resume Work Web Developer Front-End"
      },
      { charset: "utf-8" },
      { property: "og:title", content: "Eldin' Space" },
      { property: "og:site_name", content: "Eldin' Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://eldin.space" },
      {
        property: "og:image",
        content: ""
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
        this.buffer1 = 90;
        this.buffer2 = 85;
        this.buffer3 = 80;
        this.buffer4 = 80;
        this.buffer5 = 90;
        this.buffer6 = 70;
      }, 800);
    }
  }
};
</script>
<style >
</style>

