<template>
  <section v-show="isVisible">LightBox</section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {},
  props: {
    isVisible: Boolean
  }
})
</script>
