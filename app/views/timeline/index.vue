<template>
  <div>
    <h3>时间轴</h3>
    <brush-timeline :data="timelineData"></brush-timeline>
    <div style="margin-top:40px">
      <h3>时间轴2</h3>
      <brush-timeline :data="data2" render-type="json"></brush-timeline>
    </div>
  </div>
</template>
<script>
export default {
  name: 'TimelinePage',
  props: {},
  data() {
    return {
      // 注意：JavaScript Date 对象中，月份是从0开始
      timelineData: [
        {
          content:
            '<div><p class="date">2010-11-18</p><a href="" target="_blank">第一个</a></div>',
        },
        {
          content:
            '<div><p class="date">2011-11-18</p><a href="" target="_blank">新适应症</a></div>',
        },
        {
          content:
            '<div><p class="date">2014-11-18</p><a href="" target="_blank">新给药方案</a></div>',
        },
        {
          content:
            '<div><p class="date">2013-11-18</p><a href="" target="_blank">包装</a></div>',
        },
        {
          content:
            '<div><p class="date">2014-11-18</p><a href="" target="_blank">审批</a></div>',
        },
        {
          content:
            '<div><p class="date">2015-11-18</p><a href="" target="_blank">IPO</a></div>',
        },
        {
          content:
            '<div><p class="date">2016-11-18</p><a href="" target="_blank">准备上市</a></div>',
        },
        {
          content:
            '<div><p class="date">2017-11-18</p><a href="" target="_blank">上市</a></div>',
        },
      ],
      data2: [
        { date: '2012-11-18', label: 'test' },
        { date: '2017-11-18', label: 'test' },
      ],
    }
  },
  created() {},
  mounted() {},
  methods: {},
}
</script>
<style lang="scss" scoped>
</style>
