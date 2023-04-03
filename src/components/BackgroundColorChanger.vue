<template lang="">
    <div :class="[backgroundColor]">
        <button @click="changeColor">Change Color</button>
        <h1>This is a box with a dynamic background color!</h1>
    </div>
</template>

<script>
import { ref } from 'vue'
export default {
     data() {
        return {
            backgroundColor: ref('red')
        }
     },
    methods: {
        changeColor (){
            this.backgroundColor = this.backgroundColor === 'red' ? 'blue' : 'red';
        }
    },
}
</script>

<style lang="css">
   .red {
    background-color: red
   }
   .blue {
    background-color: blue
   }
</style>