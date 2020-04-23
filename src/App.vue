<template>
  <div>  
    <h1>clicked {{ timesclicked }} times</h1>
    <button @click="iAmClicked()">Click me!</button>
  </div>
</template>
 
<script>
    export default {
        data() {
            return {timesclicked:0}
        },
        props:{
          clicked:0
          },
        methods: {
            iAmClicked() {
                this.timesclicked++;
            }
        }
    };
</script>