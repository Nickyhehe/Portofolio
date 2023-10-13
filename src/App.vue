<script>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';
import skills from './components/skills.vue';

export default{
  components:{
    Header,
    skills,
    Projects,
    Contact,
    Footer
  },


}


</script>

<template>
  <body>
    <Header/>
    <skills/>
    <Projects/>
    <Contact/>
    <Footer/>

  </body>
  
</template>

<style lang="scss">
body{
  margin: 0;
  padding: 0;
  --tw-bg-opacity: 1;
  background-color: rgb(26 26 26/var(--tw-bg-opacity));
  box-sizing: border-box;
  font-family: Inter,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;
  font-size: 16px;
  scrollbar-width: thin;
  scrollbar-color: #4caf50 #f5f5f5;
}



body, html{
  scroll-behavior: smooth;
}



@media (max-width: 640px) {

}
</style>
