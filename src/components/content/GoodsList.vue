<template>
  <div class='goods-list'>
    <goods-list-item v-for="(item, index) in goods" :key="index" :goodsItem='item'></goods-list-item>
  </div>
</template>

<script>
import GoodsListItem from './GoodsListItem.vue'
export default {
  name: 'GoodsList',
  data(){
    return {}
  },
  props: {
    goods: {
      type: Array,
      default() {
        return []
      }
    }
  },
  components: {
    GoodsListItem
  },
  methods: {}
}
</script>
<style scoped>
  .goods-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
</style>
