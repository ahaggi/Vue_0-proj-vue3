<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button @click="state.count++">count is: {{ state.count }}</button>
  <p>
    Edit
    <code>components/Home.vue</code> to test hot module replacement.
  </p>
</template>


<!-- using "<script setup>" -->
<!-- To use props with <script setup> you need to call defineProps() with the component prop options as the argument-->
<!--
<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>
  -->


<!-- without "<script setup>" + with "setup()"-->
<!--
<script >
import { reactive } from "vue";
export default {
  props: {
    msg: String,
  },
  setup() {
    const state = reactive({ count: 0 });
    return {
      state,
    };
  },
};
</script>
  -->


<!-- without "<script setup>" +  Without "setup()" -->
<script >
import { reactive } from "vue";
export default {
  props: {
    msg: String,
  },
  // data: () => ({             arrow function???
  //   state: reactive({ count: 0 }),
  // }),

  data() {
    // state = reactive({ count: 0 }); // reactive is not necessary here
    return {
      state:{ count: 0 }
    };
  },
};
</script>







<style scoped>
a {
  color: #42b983;
}
</style>
