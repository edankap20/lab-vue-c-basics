<template lang="">
    <div :class="backgroundColor">
        <button @click="changeColor">Change Color</button>
        <h1>This is a box with a dynamic background color!</h1>
    </div>
</template>

<script >
import { ref } from 'vue'
export default {
     data() {
        return {
            backgroundColor: ref('red')
        }
     },
    methods: {
        changeColor (){
            if (this.backgroundColor === 'red') {
                this.backgroundColor = 'blue'
            } else {
                this.backgroundColor = 'red'
            }
        }
    },
}
</script>

<style lang="">
   .red {
    background-color: red
   } 
   .blue {
    background-color: blue
   }
</style>