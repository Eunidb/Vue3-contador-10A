<script>

    export default {
    data: () =>({
      contador: 10,
    }), 
    /*
  export default {
    data: () =>({
      return{
        contador: 200,
      };
      
    }), */

    methods: {
      saludar (){
        console.log("HOLA XD");

      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.console--;
      },
      resetear(){
        this.contador = 200;
      },
    }
  };
</script>
<template>
  <img src="./assets/logo.svg" alt="logo VUE"
  
  width="125" height="125">
 <!--
   <h1>Hola dede VUE.js 3</h1>
  <hr>
  <h2>Contador 0</h2>
  <button>+ 1</button>
  <button>- 1</button>
  <button> Reset </button>
 --> 
 
<div class="container">
  <small>
      <h1>Hola dede VUE.js</h1>
  </small>
  
  <hr>
  <h2>Contador {{contador}}</h2>
  <button @click="incrementar()"> + 1 </button>
  <button @click="decrementar()"> - 1 </button>
  <button @click="resetear()"> Reset </button>

</div>


<Style scoped>
  .container{
      text-align: center;
  }
  small{
      color: #666;
  }
  h1{
  font-weight: bolder;
  }
  h2{
      font-size: 2.5rem;
  }
  button{
      cursor: pointer;
      font-size: 1.5rem;
  }
</Style>

</template>

