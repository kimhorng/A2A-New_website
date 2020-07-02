<template>
  <v-app>
    <header>
      <NavBar/>
    </header>
    <nuxt />
  </v-app>
</template>

<script>
import NavBar from './NavBar'
export default {
  components: {
    NavBar,
  }
}
</script>

<style>
* {
  font-family: Poppins;
}
p {
  line-height: 35px;
}
li {
  line-height: 35px;
}
h2 {
  line-height: 35px;
}
h1 {
  line-height: 35px;
}
h3 {
  line-height: 35px;
}
div{
  line-height: 35px;
}
b{
  line-height: 40px;
}
</style>
