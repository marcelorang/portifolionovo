<template>
  <v-container class="fill-height" style="background: #fff">
    <v-responsive class="align-center text-center fill-height">
      <br />
      <v-row>
        <v-col cols="12" sm="6" lg="3" md="12">
          <div class="cardWrapper">
            <div class="profile-card">
              <div class="image">
                <img class="profile-img" alt="profile" src="@/assets/perfil.jpg" />
              </div>

              <div class="text-data">
                <span class="name">Marcelo Rangel</span>
                <span class="job">Desenvolvedor Jr</span>
                <span class="skills">Vue || Vuetify || Ionic || JavaScript || .NET || C#</span>
              </div>

              <div class="media-buttons">
                <a href="https://github.com/marcelorang" class="link">
                  <i class="bx bxl-github bx-border-circle" style="background: black"></i>
                </a>
                <a href="https://www.linkedin.com/in/marcelo-rangel-622089221/" class="link">
                  <i class="bx bxl-linkedin-square bx-border-circle" style="background: #0072b1"></i>
                </a>
                <a href="/CurriculoDev.pdf" class="link" download>
                  <i class="bx bxs-file-pdf bx-border-circle" style="background: #f40f02"></i>
                </a>
              </div>
              <div class="linkTittle ml-2">
                <v-row align="center">
                  <div class="ma-4">
                    <v-col cols="4" lg="4" sm="4" md="4">
                      <span>GitHub</span>
                    </v-col>
                  </div>
                  <div class="ma-4">
                    <v-col cols="4" lg="4" sm="4" md="4">
                      <span>LinkdIn</span>
                    </v-col>
                  </div>
                  <div class="ma-4">
                    <v-col cols="4" lg="4" sm="4" md="4">
                      <span>Currículo</span>
                    </v-col>
                  </div>
                </v-row>
              </div>
            </div>
          </div>
        </v-col>

        <v-col cols="12" lg="9" sm="6" md="12">
          <div>
            <h1 id="scrollToPortifolio">Portfólio</h1>
            <v-divider></v-divider>

            <v-row align="center" align-content="space-around">
              <v-col cols="12" lg="6" sm="6" md="12">
                <br />
                <h1>MedZip</h1>
                <v-carousel hide-delimiters :show-arrows="false" cycle>
                  <v-carousel-item v-for="image in images" :key="image" reverse-transition="fade-transition"
                    transition="fade-transition" contain class="darken-4" :src="image">
                  </v-carousel-item>
                </v-carousel>
                <br />

                <v-sheet class="text-left">
                  <h3>Tecnologias:</h3>
                  Vue, Vuetify, C#, .NET. <br />
                  Dashboard administrativo para clínicas médicas, odontologicas,
                  etc. Com pronto sistema de agendamento de consultas,
                  <br />cadastros de pacientes, colaboradores e médicos. <br />
                  Colaboração como desenvolvedor frontEnd.<br />
                  <p>
                    <a href="https://www.medzip.com.br">www.medzip.com.br</a>
                  </p>
                </v-sheet>
              </v-col>


              <v-col cols="12" lg="6" sm="6" md="12">
                <h1>Olho no Lance</h1>
                <v-carousel hide-delimiters :show-arrows="false" cycle>
                  <v-carousel-item v-for="image2 in images2" :key="image2" reverse-transition="fade-transition"
                    transition="fade-transition" contain class="darken-4" :src="image2">
                  </v-carousel-item>
                </v-carousel>
                <br />
                <v-col cols="12" lg="6" sm="6" md="12">
                  <v-sheet class="text-left">
                    <h3>Tecnologias:</h3>
                    Vue, Ionic, Android Stúdio .NET C# <br />
                    Aplicativo Mobile.<br />
                    Colaboração como desenvolvedor FrontEnd.
                  </v-sheet>
                </v-col>
              </v-col>


            </v-row>
          </div>
        </v-col>
      </v-row>

      <br />
      <v-card>
        <div class="text-center pa-4" style="font-size: 20px">
          Formado no curso Superior em Desenvolvimento Web pela Faculdade
          Anhanguera,<br />
          Começei no mundo da programação em agosto de 2021, quando estava
          parando de trabalhar como músico profissional por mais de quinze
          anos.<br />
          Em meio a crise da pandemia, vi que precisava migrar de carreira e foi
          onde me encontrei na área de TI. <br />
          Comprometido em adquirir conhecimentos e enfrentar desafios no
          desenvolvimento de softwares.<br />
          Buscando oportunidades para aplicar minha paixão pela tecnologia e
          construir soluções inovadoras, determinado a alcançar objetivos e
          evoluir na carreira.
        </div>
      </v-card>

      <div id="scrolltoContact">
        <v-footer>
          <div class="bg-blue-grey-lighten-5 text-center w-100">
            {{ new Date().getFullYear() }} — <strong>Marcelo Rangel</strong>
          </div>
        </v-footer>
      </div>
    </v-responsive>
  </v-container>
</template>

<script>
import img1 from "../assets/images/medzip1.png";
import img2 from "../assets/images/medzip2.png";
import img3 from "../assets/images/medzip3.png";
import img4 from "../assets/images/medzip4.png";
import img5 from "../assets/images/medzip5.png";
import img6 from "../assets/images/telaPhone12.jpg";
import img7 from "../assets/images/telaPhone13.jpg";
import img8 from "../assets/images/telaPhone14.jpg";
import img9 from "../assets/images/telaPhone15.jpg";
import img10 from "../assets/images/telaPhone16.jpg";

import curriculo from "../assets/CurriculoDev.pdf";

export default {
  data() {
    return {
      curriculum: [curriculo],
      animals: ["Column 1", "Column2", "Column 3"],
      images: [img1, img2, img3, img4, img5],
      images2: [img6, img7, img8, img9, img10],
      tab: null,
    };
  },
  methods: {
    //scrollfunction
    scrollFunction() {
      const element = document.getElementById("scrollToPortifolio");
      element.scrollIntoView({ behavior: "smooth" });
    },
    scrolltoSobre() {
      const element = document.getElementById("scrollToAbout");
      element.scrollIntoView({ behavior: "smooth" });
    },
    scrolltoContact() {
      const element = document.getElementById("scrolltoContact");
      element.scrollIntoView({ behavior: "smooth" });
    },
    downloadPdf() {
      pdfMake.createPdf(docDefinition).download("");
    },
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}

.profile-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 370px;
  width: 100%;
  background: #fff;
  border-radius: 24px;
  padding: 10px;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
  position: relative;
}

.profile-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 36%;
  width: 100%;
  border-radius: 24px 24px 0 0;
  background: #4070f4;
}

.image {
  position: relative;
  height: 150px;
  width: 150px;
  border-radius: 50%;
  background-color: #4070f4;
  padding: 3px;
  margin-bottom: 10px;
}

.image .profile-img {
  height: 100%;
  width: 100%;
  object-fit: cover;
  border-radius: 50%;
  border: 3px solid #fff;
}

.profile-card .text-data {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: #333;
}

.text-data .name {
  font-size: 22px;
  font-weight: 600;
}

.text-data .job {
  font-size: 15px;
  font-weight: 400;
}

.text-data .skills {
  margin-top: 5px;
}

.profile-card .media-buttons {
  display: flex;
  align-items: center;
  margin-top: 15px;
}

.media-buttons .link {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 34px;
  color: #fff;
  border-radius: 50%;
  margin: 0 8px;
  text-decoration: none;
  padding: 0 20px;
}

.infos {
  padding: 45px;
}

.logos-bg {
  background-image: rgb(123, 165, 166);
}

.carousel {
  width: 100%;
  position: relative;
}

.carousel-container {
  overflow: hidden;
}

.carousel-track {
  display: flex;
  width: 100%;
  transition: transform 0.3s ease-in-out;
}

.carousel-slide {
  flex: 0 0 100%;
}

.carousel img {
  width: 100%;
  height: auto;
}

.carousel-prev,
.carousel-next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  padding: 10px;
  font-size: 16px;
}

.carousel-prev {
  left: 10px;
}

.carousel-next {
  right: 10px;
}
</style>
