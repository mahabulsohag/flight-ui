<script setup lang="ts">
import { ref } from 'vue';

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <h1 class="display-1">{{ msg }}</h1>

  <div class="card">
    <button class="btn btn-md" type="button" @click="count++">
      count is {{ count }}
    </button>
  </div>
</template>
