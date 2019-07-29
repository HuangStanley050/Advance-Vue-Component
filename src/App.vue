<template>
  <div class="container">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class="row">
      <div class="col-12">
        <button @click="selectedComponent = 'Quote'">Quote</button>
        <button @click="selectedComponent = 'Author'">Author</button>
        <button @click="selectedComponent = 'New'">New Quote</button>
        <hr />
        <p>
          {{ selectedComponent }}
        </p>
        <keep-alive>
          <component :is="selectedComponent"
            ><p>
              default content
            </p>
          </component>
        </keep-alive>

        <!-- <Quote>
          <h1 slot="title">{{ quoteTitle }}</h1>
          <p slot="content">
            A Wonderful quote
          </p>
        </Quote> -->
      </div>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Quote from "./components/Quote.vue";
import Author from "./components/Author.vue";
import New from "./components/New.vue";
export default {
  name: "app",
  data: function() {
    return {
      quoteTitle: "Quote",
      selectedComponent: "Quote"
    };
  },
  components: {
    //HelloWorld
    Quote,
    Author,
    New
  }
};
</script>

<style></style>
