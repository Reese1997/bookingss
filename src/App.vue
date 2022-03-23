<template>
    <Navbar/>
  <router-view/>
  <Home/>
  <About/>
  <Services/>
  <Register/>
  <Login/>
  <Bookings/>
  <Contact/>
  <Footer/>
</template>

<script>
import Navbar from "../src/components/Navbar.vue"
import Home from "../src/components/Home.vue"
import About from './components/About.vue'
import Services from './components/Services.vue'
import Register from './components/Register.vue'
import Login from './components/Login.vue'
import Contact from './components/Contact.vue'
import Bookings from './components/Bookings.vue'
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: { Navbar, About, Services, Register, Login,
    Contact, Bookings, Footer
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
