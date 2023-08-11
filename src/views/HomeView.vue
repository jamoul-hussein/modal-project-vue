<template>
  <div class="home">
    <h1>Home</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import Signup1 from '@/components/Signup1.vue'
import Signup2 from '@/components/Signup2.vue'

export default {
  name: 'HomeView',
  components: {
    Signup1,
    Signup2
  }
}
</script>
