<template>
  <div class="toolbar">
    <div class="tool-left">
      <span v-show="isLeftIconShow">返回</span>
    </div>
    <span>首页</span>
    <div class="tool-left">
      <span v-show="isRightIconShow">更多</span>
    </div>
  </div>
</template>

<script>
/**
 * ToolBar
 */
export default {
  name: "ToolBar",
  props: {
    isLeftIconShow: {
      type: Boolean,
      default: false
    },
     isRightIconShow: {
      type: Boolean,
      default: false
    }
  },
  data() {
    return {};
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.toolbar {
  width: 100%;
  height: 4.4rem;
  background-color: #ff6e27;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.toolbar span {
  font-size: 1.8rem;
  color: #fff;
}

.tool-left {
  width: 4.4rem;
  text-align: center;
}

.tool-right {
  width: 4.4rem;
  text-align: center;
}
</style>
