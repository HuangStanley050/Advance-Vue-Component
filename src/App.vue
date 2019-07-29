<template>
  <div class="container">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class="row">
      <div class="col-12">
        <Quote>
          <h1>Quote</h1>
          <p>
            A Wonderful quote
          </p>
        </Quote>
      </div>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Quote from "./components/Quote.vue";
export default {
  name: "app",
  components: {
    //HelloWorld
    Quote
  }
};
</script>

<style></style>
