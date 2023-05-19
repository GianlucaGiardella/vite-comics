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

<style></style>
