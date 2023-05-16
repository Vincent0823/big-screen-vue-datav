<template>
  <div>
    <Chart :cdata="cdata" />
  </div>
</template>

<script>
import Chart from './chart.vue';
export default {
  data () {
    return {
      cdata: [
        {
          // 名字需要与 “common/map/fujian.js” 地图数据文件里面定义的一一对应，不能是 “福州” 或者 “闽” 之类的缩写
          name: '黄浦区',
          value: 10,
          elseData:{
            // 这里放置地图 tooltip 里想显示的数据
          }
        },
        {
          name: '徐汇区',
          value: 9,
        },
        {
          name: '长宁区',
          value: 8,
        },
        {
          name: '静安区',
          value: 7,
        },
        {
          name: '普陀区',
          value: 6,
        },
        {
          name: '虹口区',
          value: 5,
        },
        {
          name: '杨浦区',
          value: 4,
        },
        {
          name: '闵行区',
          value: 3,
        },
        {
          name: '宝山区',
          value: 2,
        }
      ]
    }
  },
  components: {
    Chart,
  },
  mounted () {
  },
  methods: {
  }
}
</script>

<style lang="scss" scoped>
</style>