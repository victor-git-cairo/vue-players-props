<template>
  <div id="app">
    <HoustonAstros class="experiment" :players="Astrosplayers" />
    <NYYankees :players="NYplayers"/>
  </div>
</template>

<script>
import HoustonAstros from "./components/HoustonAstros.vue";
import NYYankees from "./components/NYYankees.vue";

export default {
  name: "App",
  components: {
    HoustonAstros,
    NYYankees,
  },

  data() {
    return {
      Astrosplayers: [
        {
          number: "27",
          name: "Jose Altuve",
          position: "2B",
          nationality: "Venezuela",
        },
        {
          number: "23",
          name: "Michael Brantley",
          position: "LF",
          nationality: "American",
        },
        {
          number: "2",
          name: "Alex Bregman",
          position: "3B",
          nationality: "American",
        },
        {
          number: "44",
          name: "Yordan Alvarez",
          position: "DH",
          nationality: "Cuba",
        },
        {
          number: "10",
          name: "Yuli Gurriel",
          position: "1B",
          nationality: "Cuba",
        },
      ],

      NYplayers: [
        {
          number: "26",
          name: "DJ leMahieu",
          position: "1B",
          nationality: "American",
        },
        {
          number: "27",
          name: "Giancarlo Stanton",
          position: "DH",
          nationality: "American",
        },
        {
          number: "2",
          name: "Aaron Judge",
          position: "RF",
          nationality: "American",
        },
        {
          number: "29",
          name: "Gio Urshela",
          position: "3B",
          nationality: "American",
        },
        {
          number: "25",
          name: "Gleiber Torres",
          position: "SS",
          nationality: "Republica Dominicana",
        },
      ],
    };
  },
};
</script>

<style>
  #app {
    display:flex;
  }






</style>
