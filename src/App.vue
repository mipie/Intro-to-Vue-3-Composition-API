<script setup>
import { ref } from 'vue'
import socksGreenImage from './assets/images/socks_blue.jpeg'

const product = ref('Socks')
const image = ref(socksGreenImage)
const url = ref("https://google.com")

</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <a v-bind:href="url">
          <img v-bind:src="image">
        </a>
      </div>
      <div class="product-info">
        <h1>{{ product }}</h1>
      </div>
    </div>
  </div>
</template>