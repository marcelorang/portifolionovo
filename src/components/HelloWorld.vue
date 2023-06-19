<template>
  <v-tabs v-model="tab" color="deep-purple-accent-4" align-tabs="center">
    <v-tab :value="1">About</v-tab>
    <v-tab @click="scrollFunction" :value="2">Portfólio</v-tab>
    <v-tab :value="3">Contact</v-tab>
  </v-tabs>
  <v-sheet elevation="6">
    <v-container class="fill-height">
      <v-responsive class="align-center text-center fill-height">
        <br />
        <v-row>
          <v-col cols="12" sm="6" lg="3">
            <v-card variant="tonal">
              <br />
              <img
                class="profilePic"
                alt="profile"
                src="@/assets/profile.png"
              />
              <div class="infos">
                <h1>Marcelo Rangel</h1>
                <h3>Desenvolvedor Fullstack Jr</h3>
                <br />
                <h3>Vue || Vuetify || Ionic || JavaScript || .NET || C#</h3>
                <br />
                <v-row>
                  <v-col>
                    <div>
                      <a href="https://github.com/marcelorang">
                        <svg
                          width="48"
                          height="48"
                          enable-background="new 0 0 512 512"
                          id="Layer_1"
                          version="1.1"
                          viewBox="0 0 512 512"
                          xml:space="preserve"
                          xmlns="http://www.w3.org/2000/svg"
                          xmlns:xlink="http://www.w3.org/1999/xlink"
                        >
                          <g>
                            <circle cx="256" cy="256" fill="#333333" r="256" />
                            <g>
                              <path
                                d="M256,93.9c-89.5,0-162.1,72.6-162.1,162.1c0,70.5,45,130.4,107.8,152.8c0.3,0.1,1.4,0.5,1.7,0.6    c0.9,0.3,1.9,0.5,2.9,0.5c5.3,0,9.5-4.3,9.5-9.5c0-0.3,0-0.5,0-0.8l0,0c0-8.6,0-19.5,0-28.2c-10.3,2.1-25.9,4.1-34.4,0    c-11-5.3-16.6-12.1-21.9-25.5c-6.6-16.3-21.8-20.8-22.4-23.6c-0.6-2.9,16.1-7.2,24.7,2.7c8.6,9.9,17.3,29.7,35.8,27.8    c9.1-0.9,15-2.4,18.7-3.5c0.7-6.4,2.8-14.3,8.1-19.9c-43.5-7.2-72.5-30.6-72.5-76.5c0-20.9,6-37.1,16.6-49.2    c-1.8-10-4.8-33.2,3.2-41.3c0,0,11.3-7,43.7,15.8c12.1-2.8,25.5-4.2,39.8-4.2l0,0c0.3,0,0.5,0,0.8,0c0.3,0,0.5,0,0.8,0l0,0    c14.4,0.1,27.8,1.5,39.8,4.2c32.4-22.8,43.7-15.8,43.7-15.8c8,8.2,5,31.4,3.2,41.3c10.6,12.2,16.6,28.4,16.6,49.2    c0,45.9-28.9,69.3-72.5,76.5c8.3,8.7,8.6,22.8,8.6,28.6c0,5.5,0,42.3,0,42.5c0,5.3,4.3,9.5,9.5,9.5c0.8,0,1.5-0.1,2.3-0.3    c0.2,0,0.8-0.2,1-0.3c63.5-22,109.1-82.3,109.1-153.3C418.1,166.4,345.5,93.9,256,93.9z"
                                fill="#FFFFFF"
                              />
                            </g>
                          </g>
                        </svg>
                        <p>GitHub</p>
                      </a>
                    </div>
                  </v-col>
                  <v-col>
                    <div>
                      <a
                        href="https://www.linkedin.com/in/marcelo-rangel-622089221/"
                      >
                        <svg
                          width="48"
                          height="48"
                          viewBox="0 0 48 48"
                          fill="none"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            d="M0 24C0 10.7452 10.7452 0 24 0C37.2548 0 48 10.7452 48 24C48 37.2548 37.2548 48 24 48C10.7452 48 0 37.2548 0 24Z"
                            fill="#0077B5"
                          />
                          <path
                            fill-rule="evenodd"
                            clip-rule="evenodd"
                            d="M17.3188 14.8227C17.3188 16.3918 16.1377 17.6473 14.2412 17.6473H14.2064C12.3805 17.6473 11.2 16.3918 11.2 14.8227C11.2 13.2204 12.4164 12 14.277 12C16.1377 12 17.2835 13.2204 17.3188 14.8227ZM16.9605 19.8778V36.2196H11.5216V19.8778H16.9605ZM36.5752 36.2196L36.5754 26.8497C36.5754 21.8303 33.8922 19.4941 30.3131 19.4941C27.4254 19.4941 26.1325 21.0802 25.4107 22.1929V19.8783H19.9711C20.0428 21.4117 19.9711 36.22 19.9711 36.22H25.4107V27.0934C25.4107 26.605 25.446 26.1178 25.5898 25.7681C25.9829 24.7924 26.8779 23.7822 28.3805 23.7822C30.3494 23.7822 31.1365 25.2807 31.1365 27.4767V36.2196H36.5752Z"
                            fill="white"
                          />
                        </svg>
                        <p>LinkedIn</p>
                      </a>
                    </div>
                  </v-col>
                </v-row>
                <br />
                <!-- <h5>
                Comprometido em adquirir conhecimentos e enfrentar desafios no
                desenvolvimento de softwares. Buscando oportunidades para
                aplicar sua paixão pela tecnologia e construir soluções
                inovadoras. Determinado a alcançar objetivos e evoluir na
                carreira.
              </h5> -->
              </div>
            </v-card>
          </v-col>

          <v-col cols="12" lg="9" sm="6">
            <div class="text-start" style="font-size: 20px">
              Formado no curso Superior em Desenvolvimento Web pela faculdade
              Anhanguera,<br />
              Começei no mundo da programação em agosto de 2021, quando estava
              parando de trabalhar como músico profissional por mais de quinze
              anos.<br />
              Em meio a crise da Pandemia, vi que precisava migrar de Carreira e
              foi onde me encontrei no mundo da programação. <br />
              Comprometido em adquirir conhecimentos e enfrentar desafios no
              desenvolvimento de softwares.<br />
              Buscando oportunidades para aplicar sua paixão pela tecnologia e
              construir soluções inovadoras. Determinado a alcançar objetivos e
              evoluir na carreira. <br />
            </div>
          </v-col>
        </v-row>
        <br />

        <svg
          data-v-55b2ec53=""
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1442 163"
          class="logos-bg"
          fill="#e4e4e2"
        >
          <path
            data-v-55b2ec53=""
            d="m-3.90909,6l48.30303,16c48.30303,16 144.90908,48 241.51514,48c96.60606,0 193.21211,-32 289.81817,-32c96.60606,0 193.21211,32 289.81817,53.3c96.60606,21.7 193.21211,31.7 289.81817,16c96.60606,-16.3 193.21211,-58.3 241.51514,-80l48.30303,-21.3l0,160l-48.30303,0c-48.30303,0 -144.90908,0 -241.51514,0c-96.60606,0 -193.21211,0 -289.81817,0c-96.60606,0 -193.21211,0 -289.81817,0c-96.60606,0 -193.21211,0 -289.81817,0c-96.60606,0 -193.21211,0 -241.51514,0l-48.30303,0l0,-160z"
          ></path>
        </svg>

        <v-divider />
        <h1 id="scrollToPortifolio">Portfólio</h1>

        <div>
          <v-row align="center" align-content="space-between">
            <v-col cols="12" lg="6" sm="6">
              <h1>Olho no Lance</h1>
              <v-carousel hide-delimiters :show-arrows="false" cycle>
                <v-carousel-item
                  v-for="(item, i) in items"
                  :key="i"
                  :src="item.src"
                  reverse-transition="fade-transition"
                  transition="fade-transition"
                  max-height="700"
                  contain
                  class="darken-4"
                >
                </v-carousel-item>
              </v-carousel>
              <br />
              <v-sheet>
                Tecnologias: Vue, Ionic, Android Stúdio .NET C# <br />
                Aplicativo Mobile.<br />
                Colaboração FrontEnd
              </v-sheet>
            </v-col>

            <v-col cols="12" lg="6" sm="6">
              <h1>MedZip</h1>
              <v-carousel
                hide-delimiters
                :show-arrows="false"
                cycle
                max-height="700px"
              >
                <v-carousel-item
                  src="src/assets/images/medzip1.png"
                ></v-carousel-item>

                <v-carousel-item
                  src="src/assets/images/medzip2.png"
                ></v-carousel-item>

                <v-carousel-item
                  src="src/assets/images/medzip3.png"
                ></v-carousel-item>
              </v-carousel>
              <!-- <v-carousel hide-delimiters :show-arrows="false" cycle>
                <v-carousel-item
                  v-for="(item, i) in med"
                  :key="i"
                  :src="item.src"
                  reverse-transition="fade-transition"
                  transition="fade-transition"
                  max-height="700"
                  contain
                  class="darken-4"
                >
                </v-carousel-item>
              </v-carousel> -->
              <br />
              <v-sheet>
                Tecnologias: Vue, Vuetify, C#, .NET. <br />
                Dashboard Admin para clínica Médica, Odontologicas, Etc. Com
                pronto sistema de agendamento de Consultas, <br />Cadastros de
                Paciêntes, Colaboradores e médicos. <br />
                Colaboração FrontEnd.<br />
                <p><a href="https://www.medzip.com.br">www.medzip.com.br</a></p>
              </v-sheet>
            </v-col>
          </v-row>
        </div>
      </v-responsive>
    </v-container>
  </v-sheet>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      items: [
        {
          src: "/src/assets/images/telaPhone12.jpg",
        },
        {
          src: "src/assets/images/telaPhone13.jpg",
        },
        {
          src: "src/assets/images/telaPhone14.jpg",
        },
        {
          src: "src/assets/images/telaPhone15.jpg",
        },
        {
          src: "src/assets/images/telaPhone16.jpg",
        },
      ],
      // med: [
      //   {
      //     src: "src/assets/images/medzip1.png",
      //   },
      //   {
      //     src: "src/assets/images/medzip2.png",
      //   },
      //   {
      //     src: "src/assets/images/medzip3.png",
      //   },
      //   {
      //     src: "src/assets/images/medzip4.png",
      //   },
      //   {
      //     src: "src/assets/images/medzip5.png",
      //   },
      // ],
    };
  },
  methods: {
    //scrollfunction
    scrollFunction() {
      const element = document.getElementById("scrollToPortifolio");
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style>
.profilePic {
  border-radius: 50%;
  height: 150px;
}
.infos {
  padding: 45px;
}
.logos-bg {
  background-image: rgb(123, 165, 166);
}
</style>
