<template>
  <div class="app">
    <list-wrapper :data="listData" v-slot="data">
      <list-item v-for="item in data.list" :key="item.value" :data="item"></list-item>
    </list-wrapper>
  </div>
</template>

<script>
import ListWrapper from '@/components/ListWrapper'
import ListItem from '@/components/ListItem'

export default {
  name: 'app',
  data() {
    return {
      listData: [{
        name: '张大亨',
        value: 'dahengzhang'
      }, {
        name: '沈培',
        value: 'shenpei'
      }]
    }
  },
  components: {
    ListWrapper,
    ListItem
  }
}
</script>

<style lang="scss">
</style>
