<template>
  <div class="home ">
    <div class="row d-flex justify-content-center">
      <div class="card col-2">
        <div class="card-header">
       Contador
        </div>
        <div class="card-body">
          <h1>{{counter}}</h1>
        </div>
      </div>
    </div>
    <button v-on:click="increment" class="btn btn-primary m-2"> Incrementar</button>
    <button v-on:click="decrement" class="btn btn-success">Decrementar</button>
  </div>

</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increment: function (){
     this.counter++;
    },
    decrement: function(){
      this.counter--;
    }
  }
}
</script>
