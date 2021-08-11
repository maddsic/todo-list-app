<template>
<div id="app">
  <Todos v-bind:todos="todos" />
</div>
  
</template>


<script>
// importing the hello world component from the components folder.

import Todos from './components/Todos';
export default {
  name: 'app',
  components: {
    Todos
  },

// data is a function that returns an object
  data() {
    return {
      todos : [
        {
          id: 2,
          title: 'Get a wedding ring',
          completed: true 
        },
          {
          id: 2,
          title: 'Go to the tailor',
          completed: false 
        },
          {
          id: 3,
          title: 'Go to banjul and buy fabric',
          completed: false 
        }
      ]
      };
    },
  };

</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
