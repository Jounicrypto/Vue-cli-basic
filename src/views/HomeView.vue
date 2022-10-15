<template>
  <div class="home">
    <img src="logo.png" alt="logo">
    <section>
      <h1>Houses</h1>
      <button>Create One</button>
    </section>
    <section>
      <template>
        <img src="ic_search@3x.png" alt="icon-search">
   <input type="text" v-model="input" placeholder="Search for houses..." />
  <div class="item fruit" v-for="fruit in fruits" :key="fruit">
    <!-- <p>{{ fruit }}</p> -->
  </div>
  <div class="item error" v-if="input.length < 4">
     <p>No results found!</p>
  </div>
</template>
      <button>Price</button>
      <button>Size</button>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  data () {
    return {
      input: '',
      fruits: ['apple', 'banana', 'orange'],
      houses: [
        {

        }
      ]
    }
      function filteredList () {
      return fruits.filter((fruit) =>
    fruit.toLowerCase().includes(input.value.toLowerCase())
  );
}
  }

}

</script>

<style>
.home{
  text-align: center;
  text-decoration: none;

}
</style>
