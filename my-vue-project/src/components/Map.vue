<template>
  <h1>{{ latitude }} - {{ longitude }}</h1>
</template>

<script>
export default {
  data() {
    return {
      latitude: 42,
      longitude: 1729,
    };
  },
  methods: {
    getLngLat() {
      return [this.latitude, this.longitude];
    },
  },
};
</script>

<style lang="scss">
h1 {
  margin-top: 125px;
  margin-left: 3em;
}
</style>
