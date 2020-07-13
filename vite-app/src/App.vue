<template>
  <div>{{ foo }}</div>
  <div>{{ bar }}</div>
</template>

<script>
import { foo } from '@vite-symlink-test/foo'
import { bar } from '@vite-symlink-test/bar'

import { ref } from 'vue'

export default {
  name: 'App',
  setup() {
    return {
      foo: ref(foo),
      bar: ref(bar),
    }
  }
}
</script>