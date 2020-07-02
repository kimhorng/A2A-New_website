<template>
  <section id="errorpage" style="height: 100%" class="mt-xs-6 mt-sm-12 mt-12">
      <v-container>
         <v-row>
            <v-col sm="6" md="6" class="d-flex flex-column">
                  <div>
                        <p class="display-3 font-weight-bold pb-8" style="color: #535353">Oops!</p>
                        <p class="display-1">We can't seem to find page that you're looking for</p>
                        <p class="pt-8">Here are some useful links instead:</p>

                        <nuxt-link to="/about" style="text-decoration: none" class="secondary2--text">
                              <p style="margin-top: -20px">About</p>
                        </nuxt-link>
                        <nuxt-link to="/career" style="text-decoration: none" class="secondary2--text">
                              <p style="margin-top: -20px">Careers</p>
                        </nuxt-link>
                        <nuxt-link to="/blog" style="text-decoration: none" class="secondary2--text">
                              <p style="margin-top: -20px">Blog</p>
                        </nuxt-link>
                        <nuxt-link to="/news" style="text-decoration: none" class="secondary2--text">
                              <p style="margin-top: -20px">News</p>
                        </nuxt-link>
                        <nuxt-link to="/contact" style="text-decoration: none" class="secondary2--text">
                              <p style="margin-top: -20px">Contact</p>
                        </nuxt-link>
                  </div>
            </v-col>
            <v-col
                  sm="6" md="6" cols="12" class="error_image">
            </v-col>
        </v-row>
      </v-container>
  </section>
</template>

<script>
export default{
  
}
</script>

<style>
 @media screen and (max-width: 600px){
    .error_image{
      background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591021830/A2A%20Image/error_fhvsrp.jpg');
      background-size:  100%, contain, contain, cover;
      /* background-position:0% 30%, 0% 30%, center; */
      height: 400px;
    }
  }
   @media screen and (min-width: 375px){
    .error_image{
      background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591021830/A2A%20Image/error_fhvsrp.jpg');
      background-size:  100%, contain, contain, cover;
      /* background-position:0% 30%, 0% 30%, center; */
      height: 350px;
    }
  }
  @media screen and (min-width: 600px){
    .error_image{
      background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591021830/A2A%20Image/error_fhvsrp.jpg');
      background-size:  100%, contain, contain, cover; 
      background-position: center, 0% 30%, 0% 30%, center;
    }
  }
  @media screen and (min-width: 960px){
    .error_image{
      background-image: url('https://res.cloudinary.com/dgzbxayiq/image/upload/v1591021830/A2A%20Image/error_fhvsrp.jpg');
      background-size: 100%, contain, contain, cover; 
      background-position: center, 0% 30%, 0% 30%, center;
    }
  }

</style>