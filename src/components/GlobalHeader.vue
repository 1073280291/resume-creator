<template>
  <el-header height="80px" class="header-container"> {{ title }} </el-header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'GlobalHeader',
  components: {},
  props: {
    title: String,
    options: Array,
    avatar: String,
  },
  setup() {
    const user = 'abc';
    return { user };
  },
});
</script>

<style lang="less" scoped>
.header-container {
  background-color: #fff;
  color: #333;
  text-align: left;
  line-height: 80px;
}
</style>