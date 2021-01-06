<template>
  <div class="header">
    <h1>{{name}}</h1>
  </div>
</template>

<style lang="sass">
.header
  color: black
  text-align: center
  font-size: 2em
  font-family: 'Oswald', sans-serif
  font-weight: 700
  background-image: url("https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fassets.ozy.com%2Fozy-prod%2F2020%2F06%2Fshutterstock1163656021-copy.jpg%3Fwidth%3D1200%26height%3D630%26fit%3Dcover&f=1&nofb=1")

</style>

<script>
export default {
  name: 'Header',
  props: {
    name: String
  }
}
</script>
