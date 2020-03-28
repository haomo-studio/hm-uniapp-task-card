<template>
  <div class="hm-task-card">
    <div class="box">
      <text class="title">{{ options.title }}</text>
      <div class="bd">
        <div class="tagWrap">
          <text class="tag">{{ options.tag }}</text>
        </div>
        <text class="info">{{ options.info }}</text>
      </div>
      <div class="submain">
        <div class="block">
          <div class="shiliangzhinengduixiangWrap">
            <image
              class="shiliangzhinengduixiang"
              :src="options.shiliangzhinengduixiang"
            />
          </div>
          <text class="num">{{ options.num }}</text>
          <text class="minutesAgo">{{ options.minutesAgo }}</text>
        </div>
        <div class="priceWrap">
          <div class="youhuiquanWrap">
            <image class="youhuiquan" :src="options.youhuiquan" />
          </div>
          <text class="price">{{ options.price }}</text>
        </div>
      </div>
      <div class="main">
        <div class="container">
          <div class="webduanzhifuyemiantubiaoWrap">
            <image
              class="webduanzhifuyemiantubiao"
              :src="options.webduanzhifuyemiantubiao"
            />
          </div>
          <text class="confirmed">{{ options.confirmed }}</text>
        </div>
        <div class="outer">
          <div class="didianWrap">
            <image class="didian" :src="options.didian" />
          </div>
          <text class="shenzhen">{{ options.shenzhen }}</text>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmTaskCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-task-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          title: '清洁房间',
          tag: '家务活',
          info: '由 王先生 发布',
          shiliangzhinengduixiang:
            './images/img_25838_0_2.png',
          num: '2',
          minutesAgo: '分钟前',
          youhuiquan:
            './images/img_25838_0_3.png',
          price: '¥34',
          webduanzhifuyemiantubiao:
            './images/img_25838_0_1.png',
          confirmed: '已证实',
          didian:
            './images/img_25838_0_0.png',
          shenzhen: '深圳'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
