<script>
export default {
  name: "CountryComponent",
  props: [
    "name",
    "capital",
    "currency_name",
    "currency",
    "region",
    "code",
    "clickeable"
  ],
};
</script>

<template>
  <div
  >
    <h1>{{name}}</h1>
    <h2>Capital: {{capital}}</h2>
    <h3>Moneda: {{currency_name}}({{currency}})</h3>
    <h3>Region: {{region}}</h3>

  <img
      width="200"
      height="200"
      src="https://countryflagsapi.com/png/{{code}}"
    />
  </div>
</template>

<style scoped>
.country {
  padding: 2px;
  white-space: nowrap;
  width: 350px;
  height: 350px;
  border-style: solid;
  border-radius: 5px;
  border-color: grey;
}

.country-hover:hover {
  background-color: rgb(49, 49, 49);
  cursor: pointer;
}

h1 {
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>
