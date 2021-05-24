<template>
  <div id="app">
    <div class="container-scroller">
      <router-view name="header" />
    <router-view/>
  </div>
    <router-view name="footer"/>
  </div>
</template>

<script>
import Navbar from './views/layouts/Navbar'
import Footer from './views/layouts/Footer'
export default {
  name: 'App',
  components: {
    Navbar,
    Footer
  },
 

  data : function(){
    return {
      status_login: ''
    }
  }
}
</script>
