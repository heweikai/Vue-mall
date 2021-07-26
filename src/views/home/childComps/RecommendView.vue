<template>
  <div class="recommend">
    <div v-for="item in recommends" :key="item" class="recommendItem">
      <a :href="item.link">
        <img :src="item.image" alt="" />
      </a>
      <div>{{ item.title }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "RecommendView",
  props: {
    recommends: {
      type: Array,
      default() {
        return [];
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
.recommend {
  display: flex;
  text-align: center;
  width: 100%;
  font-size: 12px;
  padding: 10px 0 30px 0;
  border-bottom: 8px solid #eee;
}
.recommendItem {
  flex: 1;
}
.recommendItem img {
  width: 70px;
  margin-bottom: 10px;
}
</style>
