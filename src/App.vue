<template>
  <div id="app">
    <Nav />
    <section>
      <router-view/>
    </section>
    <Footer />
  </div>
</template>

<script>
import Nav from './components/Nav'
import Footer from './components/Footer'
export default {
  name: 'App',
  components:{
    Nav,Footer
  }
}
</script>

<style scoped>
  section{
    margin-top: 135px;
  }

  @media (max-width:768px){
    section{
      margin-top: 240px;
    }
  }
</style>