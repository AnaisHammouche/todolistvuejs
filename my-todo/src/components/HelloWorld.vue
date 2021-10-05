<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <!-- <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul> -->

<!-- <h4> TO DO LIST </h4>
<ul class="todolist">
  <li> {{ name.id(1) }} </li><br>
  <li>{{ name.id(2) }}</li><br>
  <li>{{ name.id(3) }}</li><br>
  
</ul> -->

<div class="container">
  <h1 class="">Ma Todo List</h1>
  
  <div class="card">
    <div class="card-inner">
      <ul class="list">
        <li class="list-item">
          <div class="list-item-toggle"></div><span>{{ items[0].name }} </span>
          <button class="list-item-done">DONE</button>
          <button class="list-item-delete">X</button>
          <div class="list-item-toggle"></div><span>{{ items[1].name }} </span>
          <button class="list-item-done">DONE</button>
          <button class="list-item-delete">X</button>
        </li>
      </ul>
    </div>
  </div>
</div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },

    data() {
      return {
      items: [
         {
           id: 1,
           name: 'Faire les courses',
           completed:false,
           
         },
         {
           id: 2,
           name: 'Faire du sport',
           completed: true
          
         },
      ]
    }}
  };


//   data(){
//     return {
//     todos: [{
//     id : 1,
//     name : '° Faire les courses'},
// {
//   id : 2,
//   name: '° Acheter un cadeau'},
//   {id: 3,
//   name: '° Faire du sport'}
//     ]}
//     },

  





</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
