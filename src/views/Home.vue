<template>
  <v-layout column class="mt-4 pt-2">
    <v-layout column justify-center align-center>
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

      <vue-typer class="headline" :repeat="0" text=" Gomgom Sihotang"></vue-typer>
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
        <v-card flat color="transparent" max-width="700">
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">
                <span>About</span>
                <span class="green--text">Me</span>
              </h3>
              <div>
                <p>
                  halo saya Gomgom Sihotang,
                  Saya adalah spesialis
                  <span
                    class="green--text font-weight-bold"
                  >backend enginner</span>. Saat ini saya bekerja di salah satu perusahaan
                  software house di Jakarta. Selain itu saya cukup aktif membuat konten
                  pembelajaran di youtube dan akun tiktok saya.
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
              color="green"
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
              color="green"
              :href="icon.href"
              target="_blank"
            >
              <v-icon dark>{{icon.icon}}</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
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
                </v-flex>
              </v-layout>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-flex>
    </v-layout>
    <h2 class="pl-4">
      <span>project</span>
      <span class="green--text">My</span>
    </h2>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-dialog
        v-model="project.dialog"
        lazy
        max-width="1000"
        v-for="project in projects"
        :key="project.title"
      >
        <template v-slot:activator="{ on }">
          <v-flex xs12 sm6 md4 lg4 xl4 v-on="on" >
            <v-card hover flat color="transparent"   class="m-4 p-2">
              <v-img
                :src="project.poster"
                :alt="project.title"
                width="90%"    
                lazy-src="https://cdn.dribbble.com/users/503653/screenshots/3143656/fluid-loader.gif"
              ></v-img>
              <v-card-title primary-title class="justify-center">{{project.title}}</v-card-title>
            </v-card>
          </v-flex>
        </template>
        <v-card v-if="project.dialog">
          <v-img :src="project.poster"></v-img>
          <v-card-text>
            <h3 class="headline mb-0">
              <span>Technology</span>
            </h3>
            <span v-for="(value, key) in project.tech"
             :key="key">
              <v-chip color="green" text-color="white">{{value}}</v-chip>
              <!-- <v-chip color="green" text-color="white">{{project.tech.tech2}}</v-chip> -->
            </span>
            <!-- <v-chip color="green" text-color="white">{{project.tech.tech3}}</v-chip>
            <v-chip color="green" text-color="white">{{project.tech.tech4}}</v-chip> -->
          </v-card-text>
          <v-card-actions>
            <!-- <v-btn flat large dark color="green" :href="project.git" target="_blank">
              <v-icon left>fab fa-github</v-icon>GitHub
            </v-btn> -->
            <v-btn large flat dark color="green" :href="project.demo" target="_blank">
              <v-icon left>fas fa-desktop</v-icon>Demo
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout>
    <h2 class="pl-4">
      <span>project</span>
      <span class="green--text">handle</span>
    </h2>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-dialog
        v-model="project.dialog"
        lazy
        max-width="1000"
        v-for="project in projects_office"
        :key="project.title"
      >
        <template v-slot:activator="{ on }">
          <v-flex xs12 sm6 md4 lg4 xl4 v-on="on" >
            <v-card hover flat color="transparent"   class="m-4 p-2">
              <v-img
                :src="project.poster"
                :alt="project.title"
                width="90%"
               
                
                
                lazy-src="https://cdn.dribbble.com/users/503653/screenshots/3143656/fluid-loader.gif"
              ></v-img>
              <v-card-title primary-title class="justify-center">{{project.title}}</v-card-title>
            </v-card>
          </v-flex>
        </template>
        <v-card v-if="project.dialog">
          <v-img :src="project.poster"></v-img>
          <v-card-text>
            <h3 class="headline mb-0">
              <span>Technology</span>
            </h3>

            <span v-for="(value, key) in project.tech"
             :key="key">
              <v-chip  color="green" text-color="white">{{value}}</v-chip>
              <!-- <v-chip color="green" text-color="white">{{project.tech.tech2}}</v-chip> -->
            </span>
            <div  class="mt-4 pt-2 pre-formatted" >{{ project.information }}</div>
            <!-- <v-chip color="green" text-color="white">{{project.tech.tech3}}</v-chip>
            <v-chip color="green" text-color="white">{{project.tech.tech4}}</v-chip> -->
          </v-card-text>
          <v-card-actions>
            <!-- <v-btn flat large dark color="green" :href="project.git" target="_blank">
              <v-icon left>fab fa-github</v-icon>GitHub
            </v-btn> -->
            <!-- <v-btn large flat dark color="green" :href="project.demo" target="_blank">
              <v-icon left>fas fa-desktop</v-icon>Demo
            </v-btn> -->
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout>
  </v-layout>
</template>

<script>
import { VueTyper } from "vue-typer";
import VueCompareImage from "vue-compare-image";

export default {
  metaInfo: {
    title: "Home",
    titleTemplate: "%s ← gomgom's",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      { name: "description", content: "Eldin Zaimovic's Portfolio" },
      { charset: "utf-8" },
      { property: "og:title", content: "Eldin' Space" },
      { property: "og:site_name", content: "Eldin' Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://eldin.space" },
      {
        property: "og:image",
        content: ""
      },
      { property: "og:description", content: "Eldin Zaimovic's Portfolio" }
    ]
  },
  components: {
    "vue-typer": VueTyper,
    VueCompareImage
  },
  data() {
    return {
      icons: [
        { href: "https://github.com/gomxx2", icon: "fab fa-github" },
        // {
        //   href: "https://stackoverflow.com/users/story/9660700",
        //   icon: "fab fa-stack-overflow"
        // },
        // { href: "https://twitter.com/EldinMatricar", icon: "fab fa-twitter" },
        {
          href: "https://www.linkedin.com/in/gomgom-sihotang-ab8a5b202/",
          icon: "fab fa-linkedin-in"
        },
        // {
        //   href: "https://www.xing.com/profile/Eldin_Zaimovic?sc_o=mxb_p",
        //   icon: "fab fa-xing"
        // },
        // {
        //   href: "https://www.facebook.com/EldinVasVoli",
        //   icon: "fab fa-facebook-f"
        // },
        {
          href: "https://www.youtube.com/channel/UC-IAD8yEJD-Mu6Y_56dVCtQ",
          icon: "fab fa-youtube"
        },
        // {
        //   href: "https://www.youtube.com/channel/UC-IAD8yEJD-Mu6Y_56dVCtQ",
        //   icon: "fab fa-tiktok"
        // },
        // { href: "https://www.instagram.com/matricar", icon: "fab fa-instagram" }
      ],
      projects: [
         {
          dialog: false,
          title: "ngomong.online",
          git: "",
          demo: "http://ngomong.online/",
          tech: {
            tech1: "flask",
            tech2: "python",
            tech3: "Docker",
          },
          poster: require("../../public/img/example_ngomong.png")
        },
        {
          dialog: false,
          title: "Lagu Sion",
          // git: "https://github.com/EldinZaimovic/Eldin-Space-Vue",
          demo: "https://play.google.com/store/apps/details?id=com.lagu_sion",
          tech: {
            tech1: "dart",
            tech2: "flutter",
            tech3: "Play Store Publish from Flutter",
          },
          poster: require("../../public/img/lagusion_ex.png")
        },
        {
          dialog: false,
          title: "Slapur Church Hymnal",
          git: "https://cdn.neow.in/news/images/uploaded/2018/11/1543476286_cybersecurity.jpg",
          demo: "https://play.google.com/store/apps/details?id=com.slapur_church_hymnal",
          tech: {
            tech1: "dart",
            tech2: "flutter",
            tech3: "Play Store Publish from Flutter",
          },
          poster: require("../../public/img/sch_ex.png")
        },
       
      ],
      projects_office: [
         {
          dialog: false,
          title: "Blipcom",
          git: "",
          demo: "http://ngomong.online/",
          tech: {
            tech1: "Flask",
            tech3: "Pytavia (Flask Framework)",
            tech4: "Ubuntu(Linux)",
            tech5: "Python",
            tech6: "Jinja template",
            tech7: "MongoDB",
            tech8: "Python Cherrypy",
            tech9: "JSON",
            tech10: "ChartJS",
            tech11: "Wordpress",
            tech12: "AJAX",
            tech13: "Apache",
            tech14: "rest API"
          },
          information: "BLIPCOM is an agile technology services company providing Managed Services, IT solutions, Consultancy\nand highly integrated online platforms that support learning & talent in organisationsn \n \
          Project Key Roles: \n \
          - Develop mobile API with python - REST API Scheduler MRT Jakarta \n \
          - Develop clients website ( Back-End ) - CMS MRT Jakarta",
          poster: require("../../public/img/blipcom_ex.png")
        },
        {
          dialog: false,
          title: "CRM Barantum",
          // git: "https://github.com/EldinZaimovic/Eldin-Space-Vue",
          demo: "https://play.google.com/store/apps/details?id=com.lagu_sion",
          tech: {
            tech1: "Lumen",
            tech2: "Vue",
            tech3: "Lumen (PHP framework)",
            tech4: "vue (frontend framwork)",
            tech5: "Javascript",
            tech6: "LDAP",
            tech7: "Elastic Search",
            tech8: "CSS",
            tech9: "HTML",
            tech10: "Bootstrap",
            tech11: "MySQL",
            tech12: "Apache",
            tech13: "PHP",
            tech14: "Sendinblue",
            tech15: "JSON",
            tech16: "rest API"
          },
          information: "Barantum.com is offering its services in CRM and IP-PBX development since 2017. And ever since its inception it has aspired to be the best services.\nThey have been working day and night to ensure that every small to medium sized business is able to offer their customers with the best service possible. \n \
          Project Key Roles:\n \
          - Develop CRM system \n \
          - Develop API ( Back-End ) using PHP/LUMEN \n \
          - Develop UX using vue framework, JS, HTML, CSS (Front-End) \n \
          - handle system flow (Frontend & Backend) \n \
          - integrated system with outside api provider \n \
          - handle client requests \n \
          - Helping other stuff in application development (Front-End or Back-End Programming, Guiding new developer)",
          poster: require("../../public/img/barantum_ex.png")
        },
        {
          dialog: false,
          title: "PMB Unai",
          git: "https://cdn.neow.in/news/images/uploaded/2018/11/1543476286_cybersecurity.jpg",
          demo: "https://play.google.com/store/apps/details?id=com.slapur_church_hymnal",
          tech: {
            tech1: "Laravel",
            tech2: "PHP",
            tech3: "Laravel (PHP framework)",
            tech4: "Jquery",
            tech5: "Javascript",
            tech6: "CSS",
            tech7: "HTML",
            tech8: "Bootstrap",
            tech9: "MySQL",
            tech10: "Apache",
            tech11: "PHP"
          },
          poster: require("../../public/img/pmb_ex.png")
        },
       
      ],
      text1: ["Full-Stack Developer", "Backend Engineer", "Trainer"],
      leftImage: require("../../public/img/1.png"),
      rightImage:require( "../../public/img/3.png"),
      // leftImage2: require("../../public/img/3.png"),
      // rightImage2: require("../../public/img/2.png"),
      // leftImage: "https://i.xx.com/bU50uS9.jpg",
      // rightImage: "https://i.xx.com/z3ZoEEw.jpg",
      // leftImage2: "https://i.xx.com/z3ZoEEw.jpg",
      // rightImage2: "https://i.xx.com/Dcz2PGx.jpg",
      sliderLine: 0,
      hSize: 0,
      sliderPosition: 0.5
    };
  }
};
</script>
<style>
.pre-formatted {
  white-space: pre;
}

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
}
.vue-typer .custom.char.typed {
  color: green;
}
.vue-typer .custom.char.selected {
  color: #e91e63;
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

