<template>
  <div class="backdrop">
    <div class="modal" :class="{ sale: theme === 'sale'}">
        <h1>{{ header }}</h1>
        <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>

export default {
    props: ['header', 'text', 'theme'],
    methods: {
        handle(){
            console.log(this.theme)
        }
    }
}

</script>


<style scoped>
.modal {
  width: 300px;
  padding: 20px;
  margin: 115px auto;
  border-radius: 8px;
  background: white;
}
.backdrop {
  top: 0;
  position: fixed;
  background: rgba(0, 0, 0, 0.438);
  width: 100%;
  height: 100%;
}

.sale {
    background: rgb(250, 101, 101);
}
</style>
