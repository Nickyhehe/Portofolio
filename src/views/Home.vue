<template>
    <body>
        <Header/>
        <Projects/>
        <Contact/>
        <Footer/>
    
      </body>
      
</template>

<script>
import Header from './components/Header.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

export default{
  components:{
    Header,
    Projects,
    Contact,
    Footer
  }

}

</script>


<style>

</style>