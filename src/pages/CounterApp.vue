<template>
  <NavBar />
  <section>
    <h1 className="title">Simplified Counter App!</h1>
    <div className="info">
      <p>
        Increase, Decrease, Set A Value and Reset.
      </p>
    </div>
    <div className="count">Count: {{count}}</div>
    <div className="card">
      <div>
        <input class="input-field" type="number" v-model="value" />
        <input class='submit' type='submit' @click='setValue(value)' value='Set Value'>
      </div>
      <button className="button" @click="increment">
        +
      </button>
      <button 
      className="button" @click="decrement">
        -
      </button>
      <button className="reset" @click="reset">
        Reset
      </button>
    </div>
  </section>
  <Footer />
</template>

<script>
  import useCounter from '@/composables/counter'
  import { NavBar, Footer } from "../components";
  
  export default {
    setup() {
      const { count, increment, decrement, reset, setValue } = useCounter()
  
      return {
        count,
        increment,
        decrement,
        reset,
        setValue,
        value: 0,
      }
    },
    components: {
    NavBar, Footer
  }
  }
  </script>