<template>

    <Navbar/>

  <Home/>
  <About/>
  <Services/>
  <Register/>
  <Login/>
  <Bookings/>
  <Contact/>
  <Footer/> 
   <!-- <router-view/> -->
</template>

<script>
import Navbar from '../src/components/Navbar.vue'
import Home from '../src/components/Home.vue'
import About from '../src/components/About.vue'
import Services from '../src/components/Services.vue'
import Register from '../src/components/Register.vue'
import Login from '../src/components/Login.vue'
import Contact from '../src/components/Contact.vue'
import Bookings from '../src/components/Bookings.vue'
import Footer from '../src/components/Footer.vue'

export default {
  name: "App",
  components: { Navbar, About, Services, Register, Login,
    Contact, Bookings, Footer, Home
  }
}
</script>

<style scoped>
#app {
 font-family: 'Bebas Neue', cursive;
font-family: 'League Gothic', sans-serif;
font-family: 'Smooch Sans', sans-serif;  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
