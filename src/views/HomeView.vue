//template es el html
<template>
  <div class="home">
    <img alt="Shop logo" src="../assets/shop-in-shop-salesland.png">
    <HelloWorld msg="Welcome to my shop online!"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HelloHome from '@/components/HelloWorld.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'HomeView',
  components: {
    HelloHome,
  },
});
</script>
