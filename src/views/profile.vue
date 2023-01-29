//template es el html
<template>
  <div class="home">
    <img alt="Shop logo" src="../assets/shop-in-shop-salesland.png">
    <HelloWorld msg="Welcome to my shop online!"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';


export default defineComponent({
  name: 'HomeView',
  components: {
    Hello,
  },
});
</script>