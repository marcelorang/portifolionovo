<template>
  <v-col cols="12" lg="9" sm="6">
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
  </v-col>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "src/assets/images/telaPhone12.jpg",
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
    };
  },
};
</script>
