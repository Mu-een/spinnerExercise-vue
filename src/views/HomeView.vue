<template>
 <NavBar />
 <HelloWorld />
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import NavBar from '@/components/NavBar.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    NavBar
  }
}
</script>
