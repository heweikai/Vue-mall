<template>
  <div class="nav-bar">
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {};
  },
  methods: {}
};
</script>

<style>
.nav-bar {
  display: flex;
  line-height: 44px;
  height: 44px;
  box-shadow: 0 5px 10px rgba(100, 100, 100, 0.1);
}
.left,
.right {
  width: 60px;
}
.center {
  flex: 1;
  text-align: center;
  font-weight: 400;
  font-size: 18px;
  color: #dfe6e9;
}
</style>
