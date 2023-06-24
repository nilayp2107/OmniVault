<template>
  <nav class="navbar">
    <ul class="navbar-nav">
      <li class="nav-item" v-for="(link, index) in links" :key="index">
        <router-link :to="link.url" class="nav-link">
          <span v-if="link.text === 'Cart'">
            <i class="fas fa-shopping-cart"></i>
            <span class="cart-count">{{ count }}</span>
          </span>
          <span v-else>{{ link.text }}</span>
        </router-link>
      </li>
    </ul>
  </nav>
</template>
  
<script>
export default {
name: 'NavBar',
props: {
    count : Number
},
data() {
    return {
    links: [
        { url: '/', text: 'OMNIVAULT' },
        { url: '/about', text: 'About Us' },
        { url: '/contact', text: 'Explore' },
        { url: '/profile', text: 'Profile' },
        { url: '/cart', text: 'Cart' }
    ]
    };
}
};
</script>
  
<style>
.navbar {
background-color: #f2f2f2;
padding: 10px;
}

.navbar-nav {
list-style-type: none;
padding: 0;
margin: 0;
display: flex;
}

.nav-item {
margin-right: 10px;
}

.nav-link {
text-decoration: none;
color: #333;
padding: 5px;
border-radius: 3px;
}

.nav-link:hover {
background-color: #ccc;
}

.cart {
position: relative;
display: block;
width: 28px;
height: 28px;
height: auto;
overflow: hidden;
.material-icons {
position: relative;
top: 4px;
z-index: 1;
font-size: 24px;
color: rgb(9, 9, 9);
}
.count {
position: absolute;
top: 0;
right: 0;
z-index: 2;
font-size: 11px;
border-radius: 50%;
background: #d60b28;
width: 16px;
height: 16px;
line-height:16px;
display: block;
text-align: center;
color: rgb(3, 3, 3);
font-family: 'Roboto', sans-serif;
font-weight: bold;
}
}

</style>
  