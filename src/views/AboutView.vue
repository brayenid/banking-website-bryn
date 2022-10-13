<style scoped>
ol {
  margin-left: 30px;
}
.hide {
  opacity: 0;
  transition: 0.3s;
  transform: translateY(100px);
}
.show {
  opacity: 1;
  transform: translateY(0);
}
</style>

<template>
  <ol class="hide">
    <li v-for="data in datas" :key="data.id">
      {{ data.title }} - <strike>{{ data.price }} </strike>({{ Math.round(data.price - data.price * (data.discountPercentage / 100)) }})
    </li>
  </ol>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import axios from 'axios'

const datas = ref([])
const getData = async () => {
  const products = await axios.get('https://dummyjson.com/products')
  datas.value = products.data.products.slice(1, 11)
}
onMounted(() => {
  getData()
  setTimeout(() => {
    document.querySelector('.hide').classList.add('show')
  }, 1000)
})
</script>
