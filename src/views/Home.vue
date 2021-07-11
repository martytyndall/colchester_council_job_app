<template>
  <div class="home container">
    <Header title="Marty Tyndall" heading="I am applying for the role of Web 
        Developer at Colchester Borough Council." />

      <AboutMe />
      <HomeAsideBox />    
        
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header'
import AboutMe from '@/components/AboutMe'
import HomeAsideBox from '@/components/HomeAsideBox'

export default {
  name: 'Home',
  components: {
    Header,
    AboutMe,
    HomeAsideBox,
  }
}
</script>

<style>

@media screen and (max-width: 592px) {
  
}

@media screen and (max-width: 592px){
        .about-me{
          width: 100%;
        }

        .home-aside1{
            width: 100% !important;
            height: 140px;
            margin-top: 40px;
        }

        .home-aside1 * {
          float: left;
        }

        .home-aside2{
            width: 100% !important;
        }

        .img-box{
          margin: 0 auto;
        }
        
    }
  
</style>

