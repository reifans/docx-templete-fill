<template>
  <div class="btn" @click="print">按钮</div>
</template>

<script>
import { exportDocx } from '@/utils/docx.js'
export default {
  components: {},
  data() {
    return {};
  },
  computed: {},
  watch: {},
  methods: {
      print() {
          exportDocx('/templete.docx', {userName: '鸡汤'}, '模版.docx')
      }
  },
  created() {},
  mounted() {},
};
</script>

<style  scoped>
.btn {
    width: 50px;
    height: 50px;
    background-color: pink;
}
</style>