<template>
  <p>{{ name }}</p>
  <button @click="changeName('zelda')"></button>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  components: {},
  data() {
    return {
      name: 'Link',
      age: 25 as number | string,
    }
  },
  methods: {
    changeName(name: string) {
      this.name = name;
    }
  }
});
</script>
