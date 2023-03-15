<template>
  <LightBoxImage :is-visible="lightBoxOpened" />
  <HeaderComponent />
  <AddToCartButton />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HeaderComponent from './components/HeaderComponent.vue'
import LightBoxImage from './components/LightBoxImage.vue'
import AddToCartButton from './components/buttons/AddToCartButton.vue'

export default defineComponent({
  components: {
    HeaderComponent,
    AddToCartButton,
    LightBoxImage
  },
  data() {
    return {
      lightBoxOpened: true
    }
  }
})
</script>

<style scoped></style>
