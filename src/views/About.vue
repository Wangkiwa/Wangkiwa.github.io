<template>
  <div class="about">
    <div class="title">2024年部分考生初试成绩查询</div>
    <section>
      <ul>
        <li>
          <div class="left">姓名</div>
          <div class="right">潘璐瑶</div>
        </li>
        <li>
          <div class="left">报名号</div>
          <div class="right">220773631</div>
        </li>
        <li>
          <div class="left">准考证号</div>
          <div class="right">102004211819908</div>
        </li>
        <li>
          <div class="left">总分</div>
          <div class="right">357</div>
        </li>
        <li>
          <div class="left">第一门</div>
          <div class="right">(101)思想政治理论：65</div>
        </li>
        <li>
          <div class="left">第二门</div>
          <div class="right">(201)英语（一）：60</div>
        </li>
        <li>
          <div class="left">第三门</div>
          <div class="right">(618)戏剧与影视艺术理论: 102</div>
        </li>
        <li>
          <div class="left">第四门</div>
          <div class="right">(808)戏剧与影视专业基础：130</div>
        </li>
        <li>
          <div class="left">备注:</div>
          <div class="right">无</div>
        </li>
      </ul>
    </section>
    <footer>
      <img src="../assets/image/3232.jpg" width="100%" height="100px" />
    </footer>
    <div class="re" @click="back">返回</div>
  </div>
</template>

<script>
export default {
  // 组件名称
  name: "about",
  // 局部注册的组件
  components: {},
  // 组件参数 接收来自父组件的数据
  props: {},
  // 组件状态值
  data() {
    return {};
  },
  // 计算属性
  computed: {},
  // 侦听器
  watch: {},
  // 生命周期钩子   注：没用到的钩子请自行删除
  /**
   * 组件实例创建完成，属性已绑定，但DOM还未生成，el属性还不存在
   */
  created() {},
  /**
   * el 被新创建的 vm.el 替换，并挂载到实例上去之后调用该钩子。
   * 如果 root 实例挂载了一个文档内元素，当 mounted 被调用时 vm.el 也在文档内。
   */
  mounted() {},
  // 组件方法
  methods: {
    back() {
      this.$router.back();
    },
  },
};
</script>

<style scoped lang="less" scoped>
.title {
  width: 100%;
  height: 48px;
  background-color: #4a92e3;
  color: #fff;
  font-size: 18px;
  display: flex;
  justify-content: center;
  align-items: center;
}

ul {
  li {
    width: 100%;
    height: 54px;
    display: flex;
    padding-left: 20px;
    border-bottom: 1px solid #ececec;
    background-color: #fff;

    .left {
      line-height: 54px;
      width: 80px;
      height: 54px;
      // background-color: pink;
      font-size: 20px;
    }

    .right {
      width: auto;
      height: 54px;
      margin-left: 20px;
      line-height: 54px;
      color: rgb(102, 102, 102);
      font-size: 17px;
    }
  }
}

footer {
  margin-top: 10px;
  padding: 0 15px;
}

.re {
  width: 345px;
  height: 47px;
  background-color: #4a92df;
  font-size: 20px;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
  margin-left: 10px;
}
</style>
