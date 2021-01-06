<template>
  <div class="home">
    <div class="header">
      <Header class="h" name="Radiohead" />
    </div>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/albums">Albums</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <figure class="members">
      <img class="them" src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F3w8dlo2orf8y3crtc22sslbh-wpengine.netdna-ssl.com%2Fwp-content%2Fuploads%2F2020%2F02%2FWebp.net-resizeimage-18.jpg&f=1&nofb=1" alt="radiohead">
    </figure>
    <p class="names">
      <a href="https://en.wikipedia.org/wiki/Colin_Greenwood">Colin Greenwood</a>,
      <a href="https://en.wikipedia.org/wiki/Jonny_Greenwood">Jonny Greenwood</a>,
      <a href="https://en.wikipedia.org/wiki/Thom_Yorke">Thom Yorke</a>,
      <a href="https://en.wikipedia.org/wiki/Philip_Selway">Philip Selway</a>,
      <a href="https://en.wikipedia.org/wiki/Ed_O%27Brien">Ed O'Brien</a>
    </p>
  </div>
</template>


<style lang="scss" scoped>
.header {
  position: relative;
  margin: 0;
}

#nav {
  padding: 30px;
  text-align: center;

  a {
    font-size: 1.3em;
    font-weight: bold;
    color: #D3D3D3;

    &.router-link-exact-active {
      color: #B60F32;
}
}
a:hover {
  color: #B60F32;
}
}

.members {
  display: flex;
  justify-content: center;
  .them {
    max-width: 100%;
  }
}

.names {
  text-align: center;
  a {
    color: #D3D3D3;
    text-decoration: underline;
}
a:hover {
  color: #B60F32;
}
}
</style>

<script>
import Header from "@/components/Header";

export default {
  name: 'Home',
  components: {
    Header
  }
}
</script>
