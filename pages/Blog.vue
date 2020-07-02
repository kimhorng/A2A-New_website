<template>
  <div>
    <section>
      <!-- <v-container class="mt-12">
      <div class="display-1">Blog Page Coming soon..</div>
    </v-container> -->
      <CSoon />
    </section>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Footer from '../layouts/Footer'
import CSoon from '../layouts/ComingSoon'
export default {
  components: {
    Footer,
    CSoon
  }
}
</script>

<style lang="scss" scoped></style>
