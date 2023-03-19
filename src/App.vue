<template>
  <HeaderComponent />
  <LightBoxImage :is-visible="lightBoxOpened" />
  <AddToCartButton />
  <CartComponent />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HeaderComponent from './components/HeaderComponent.vue'
import LightBoxImage from './components/LightBoxImageComponent.vue'
import CartComponent from './components/cart/CartComponent.vue'
import AddToCartButton from './components/buttons/AddToCartButton.vue'

export default defineComponent({
  components: {
    HeaderComponent,
    AddToCartButton,
    LightBoxImage,
    CartComponent
  },
  data() {
    return {
      lightBoxOpened: true
    }
  }
})
</script>

<style scoped></style>
