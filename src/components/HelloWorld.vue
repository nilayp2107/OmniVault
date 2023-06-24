<template>
    <h1>{{ msg }}</h1>
    <p>OmniVault is an all-inclusive e-commerce platform that offers a wide 
      variety of products to customers worldwide.This repository 
      contains the codebase for the OmniVault web application, 
      built with modern technologies such as Vue.js, Node.js and MongoDB. 
      It provides a seamless shopping experience with 
      features like product search, cart management, secure checkout, and order tracking. 
      Join us in revolutionizing the way people shop online with OmniVault.</p>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
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
