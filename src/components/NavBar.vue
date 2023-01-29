<template>
    <nav>
        <a href="@/components/LogIn.vue" target="_blank">Login</a>
        <a href="@/views/productsList.vue" target="_blank">Products</a>
    </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'navBar',
  props: {
    msg: String,
  },
});
</script>
