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
          <ul class="series-list">
            <SeriesCard
              v-for="card in SeriesArr"
              :seriesImage="card.thumb"
              :seriesTitle="card.series"
              :key="card.series"
            />
          </ul>
          <button class="more">load more</button>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.container-bg {
  background-color: #1c1c1c;
}

.jumbotron {
  height: 400px;
  width: 100%;
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
}

.container {
  width: 960px;
  max-width: 1280px;
  margin: 0 auto;
}

.current-series {
  width: 100%;
  padding: 2.5rem 0 1rem;
  position: relative;
  text-align: center;
  color: white;
}

.current-series {
  h2 {
    font-size: 1.2rem;
    padding: 0.5rem 1rem;
    transform: translateY(-50%);
    position: absolute;
    top: 0;
    left: 0;
    text-transform: uppercase;
    background-color: #0282f9;
  }
  .series-list {
    width: 100%;
    height: 400px;
    margin-bottom: 2rem;
    display: grid;
    grid-template-columns: repeat(6, minmax(0, 1fr));
    grid-template-rows: repeat(2, 1fr);
    row-gap: 2rem;
  }

  .more {
    padding: 0.5rem 2.5rem;
    font-weight: 600;
    color: white;
    text-transform: uppercase;
    border: unset;
    background-color: #0282f9;
  }

  .more:hover {
    cursor: pointer;
  }
}
</style>
