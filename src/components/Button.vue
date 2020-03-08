<template>
  <div>
    <button v-on:click = increment()>+</button>
            <button v-on:click = decrement()>-</button>
            <p v-html = "counter"></p>
  </div>
</template>

<script>
export default {
  
  data(){
    return{
        counter: 0
        }
  },
  methods : {
      increment:function() {
          this.counter = this.counter + 1;
      },

      decrement:function() {
          this.counter = this.counter - 1;
      }
  }
}
</script>