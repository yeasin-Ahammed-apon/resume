<template>
  <div class="home">
    <div class="container-fluid p-0">
      <about/>
      <!-- <exp/> -->
      <education/>
      <skills/>
      <projects/>
      <hobby/>
      <!-- <award/> -->
    </div>
  </div>
</template>

<script>
import About from '../components/home/About.vue'
// import Award from '../components/home/Award.vue'
import Education from '../components/home/Education.vue'
// import Exp from '../components/home/Exp.vue'
import Hobby from '../components/home/Hobby.vue'
import Projects from '../components/home/Projects_demo.vue'
import Skills from '../components/home/Skills.vue'
export default {
  name: 'Home',
  components: {
    About,
    // Award,
    Education,
    // Exp,
    Hobby,
    Projects,
    Skills,
    
  }
}
</script>
