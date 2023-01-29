<template>
    <nav>
        <div class="title">
            <h4>{{ title }}</h4>
        </div>
        <div class="links" v-if="links">
            <button
        v-for="link in links"
        :key="link.label"
        @click="onClick(link)"
        class="btn btn-primary"
      >
        {{ link.label }}
      </button>
      <button @click="changeGreeting">Cambiar estado</button>
      <button @click="toggleCart" class="btn btn-secondary">Carrito</button>
    </div> 


            href="@/components/LogIn.vue" target="_blank">Login</a>
            <a href="@/views/productsList.vue" target="_blank">Products</a>
        </div>
    </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'NavBar',
  props: {
    title: String,
    required: true,
  },
});
</script>

<style scoped>
nav {
    width: 100%;
    display: flex;
    justify-content: space-between;
    background-color: aquamarine;
  }
  
.links {
    padding: 20%;
}

  nav a {
    font-weight: bold;
    color: #2c3e50;
  }
  
  nav a.router-link-exact-active {
    color: #42b983;
  }
</style>
