<template>
  <div>
    <img :src="comicImg" alt="" />
    <h3>{{ comicName }}</h3>
  </div>
</template>

<script>
export default {
  props: {
    comicImg: String,
    comicName: String,
  },
};
</script>

<style>
</style>