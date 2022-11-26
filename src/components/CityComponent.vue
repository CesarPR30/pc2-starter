<script>
export default {
  name: "CityComponent",
  props: [
    "name",
    "country_name",
    "country_code",
    "state_name",
    "latitude",
    "longitude",
    "code",
  ],
};
</script>

<template>
  <div
  >
    <h1>{{ name }}</h1>
    <h2>Pais: {{ country_name }}({{ country_code }})</h2>
    <h3>Estado: {{ state_name }}</h3>
    <h3>Latidud: {{ latitude }}</h3>
    <h3>Longitud: {{ longitude }}</h3>
    <img
      width="200"
      height="200"
      src:=" '../src/assets/city.jpg.' "
    />
  </div>
</template>

<style scoped>
.city {
padding: 2px;
white-space: nowrap;
width: 350px;
height: 350px;
border-style: solid;
border-radius: 5px;
border-color: grey;
}
h1 {
overflow: hidden;
text-overflow: ellipsis;
}
</style>
