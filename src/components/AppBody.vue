<script>
import SeriesArrJson from "../assets/json/dc-comics.json";
import SeriesCard from "./Card.vue";

export default {
  data() {
    return {
      SeriesArr: SeriesArrJson,
    };
  },
  components: { SeriesCard },
};
</script>

<template>
  <main>
    <div class="container-bg">
      <div class="jumbotron"></div>
      <div class="container">
        <div class="current-series">
          <h2>current series</h2>
          <ul>
            <SeriesCard
              v-for="card in SeriesArr"
              :seriesImage="card.thumb"
              :seriesTitle="card.series"
              :key="card.series"
            />
          </ul>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.container-bg {
  background-color: #1c1c1c;
}

.container {
  width: 960px;
  max-width: 1280px;
  height: 100px;
  margin: 0 auto;
}

.container {
  div {
    height: 100%;
    display: grid;
    align-content: center;
    font-size: 2.5rem;
    color: white;
  }
}
</style>
