<script>
export default {
  props: {
    seriesImage: String,
    seriesTitle: String,
    key: String,
  },
};
</script>

<template>
  <li :key="key">
    <img :src="seriesImage" :alt="seriesTitle" />
    <h2>{{ seriesTitle }}</h2>
  </li>
</template>

<style lang="scss" scoped>
li {
  padding-inline: 0.7rem;
  display: flex;
  flex-direction: column;
  gap: 1.2rem;
  text-align: start;
}

li {
  img {
    width: 100%;
    height: 140px;
    object-fit: cover;
    object-position: top;
  }

  h2 {
    font-size: 0.6rem;
    font-weight: 400;
    text-transform: uppercase;
    line-height: 0.8rem;
  }

  img:hover,
  h2:hover {
    cursor: pointer;
  }
}
</style>
