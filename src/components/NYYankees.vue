<template>
  <div class="player-list">
    <h2>NewYork Yankees Rosters</h2>
    <!--  <h3>Batters</h3> -->
    <!-- <ul>
      <li></li>
    </ul> -->
    <!-- <h3>Pitchers</h3> -->
    <ul v-for="player in players" :key="player.number">
      <li>
        <p>{{ player.name }}</p>
        <p>{{ player.position }}</p>
        <p>{{ player.nationality }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NYYankees",
  props: ["players"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  display: block;
}

.player-list {
  background: lightskyblue;
  padding: 10px 20px;
  /* height: 75px; */
  /* width: 400px; */
  margin: 10px;
}

.player-list ul {
  list-style-type: none;
}

ul li {
  text-align: left;
}

li p {
  display: inline-block;
  padding-right: 15px;
  margin: 0px;
}
</style>
