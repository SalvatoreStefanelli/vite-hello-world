<script>
export default {
  name: "App",
  data() {
    return {
      message: "Salvatore",
      content: "lorem ipsum dolor",
      msg: "lorem",
      name: " ",
      lastname: " ",
    }
  },
  methods: {
    testFunction() {
      console.log('This is function');
    }
  }
};
</script>

<template>
  <header>
    <h1>Hello {{ message }}</h1>
    <p>{{ content }}</p>
    <input type="text" v-model="msg">
    <div>
      <label for="name">First name</label>
      <input type="text" v-model="name">
      <label for="lastname">Last name</label>
      <input type="text" v-model="lastname">
      <p>Ciao {{ name }} {{ lastname }}</p>
    </div>

    <button @click="testFunction">Click me</button>
  </header>
</template>

<style>
body {
  background-color: blue;
}

header {
  background-color: orange;
}

h1 {
  color: green;
}
</style>
