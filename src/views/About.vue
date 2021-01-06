<template>
  <div class="about">
    <p class="text">
      Radiohead are an English <a href="https://en.wikipedia.org/wiki/Rock_music">rock</a>
      band formed in <a href="https://en.wikipedia.org/wiki/Abingdon-on-Thames">Abingdon</a>,
      <a href="https://en.wikipedia.org/wiki/Oxfordshire">Oxfordshire</a>, in 1985.
      The band consists of <a href="https://en.wikipedia.org/wiki/Thom_Yorke">Thom Yorke</a>
      (vocals, guitar, piano, keyboards),
      brothers <a href="https://en.wikipedia.org/wiki/Jonny_Greenwood">Jonny Greenwood</a>
      (lead guitar, keyboards, other instruments)
      and <a href="https://en.wikipedia.org/wiki/Colin_Greenwood">Colin Greenwood</a>
      (bass), <a href="https://en.wikipedia.org/wiki/Ed_O%27Brien">Ed O'Brien</a> (guitar, backing vocals)
      and <a href="https://en.wikipedia.org/wiki/Philip_Selway">Philip Selway</a> (drums, percussion).
      They have worked with producer <a href="https://en.wikipedia.org/wiki/Nigel_Godrich">Nigel Godrich</a>
      and cover artist <a href="https://en.wikipedia.org/wiki/Stanley_Donwood">Stanley Donwood</a> since 1994.
      Radiohead's <a href="https://en.wikipedia.org/wiki/Experimental_music">experimental</a>
      approach is credited with advancing the sound of
      <a href="https://en.wikipedia.org/wiki/Alternative_rock">alternative rock</a>.
    </p>

    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/albums">Albums</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  </div>
</template>

<style lang="sass" scoped>

.about
  height: 100vh
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  min-height: 100%
  position: relative

  .text
    overflow: scroll
    max-height: 50vh
    width: 50vw
    color: #D3D3D3
    font-size: large
    font-weight: 700
    text-align: left
    a
      color: #D3D3D3
      font-style: italic
    a:hover
      color: #B60F32

#nav
  position: absolute
  padding-bottom: 20px
  width: 100%
  text-align: center
  bottom: 0

  a
    font-size: 1.3em
    font-weight: bold
    color: #D3D3D3

    &.router-link-exact-active
      color: #B60F32
  a:hover
    color: #B60F32

</style>

<script>
export default {
  name: 'About'
}
</script>
