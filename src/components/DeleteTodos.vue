<template>
  <div>
    <ul>
      <li v-for="todo in todos" :key="todo.id">
        {{ x }}
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  name: `DeleteTodos`,
  computed: {
    delete() {
      return this.$store.getters.count;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  // display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
