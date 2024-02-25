<template>
  <div class="home">
    <header>
      <div class="logo"><img src="@/assets/image/yzw logo.png" /></div>
      <div class="add">
        <img src="@/assets/image/头像.png" />
        <img src="@/assets/image/导航.png" />
      </div>
    </header>
    <div class="title">2024年部分考生初试成绩查询</div>
    <div class="notice">姓名、证件号码、准考证号必填</div>
    <section>
      <ul>
        <li>
          <div class="left">
            <i style="color: red; margin-right: 2px">*</i>姓名
          </div>
          <div class="right"><input type="text" placeholder="请输入" /></div>
        </li>
        <li>
          <div class="left">
            <i style="color: red; margin-right: 2px">*</i>证件号码
          </div>
          <div class="right"><input type="text" placeholder="请输入" /></div>
        </li>
        <li>
          <div class="left">
            <i style="color: red; margin-right: 2px">*</i>准考证号
          </div>
          <div class="right"><input type="text" placeholder="请输入" /></div>
        </li>
        <li>
          <div class="left">
            <i style="color: red; margin-right: 2px">*</i>报考单位
          </div>
          <div class="right" style="margin-right: 95px">(10355)江南大学</div>
        </li>
      </ul>
    </section>
    <div class="js">
      本系统所有数据均为招生单位提供,招生单位对查询结果负责解释
    </div>
    <div class="search"><button @click="search">查询</button></div>
    <footer class="footer">
      <p>
        主办单位：教育部学生服务与素质发展中心<br />
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;（原全国高等学校学生信息咨询与就业指导)
      </p>
      <p>Copyright &copy 2003-2024 学信网 All Rights Reserved</p>
      <!-- <img
        src="../assets/image/底部.jpg"
        width="100%"
        height="100px"
        style="margin-top: 93px"
      /> -->
    </footer>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    search() {
      this.$router.push("/About");
    },
  },
};
</script>
<style lang="less" scoped>
header {
  width: 100%;
  height: 53px;
  background-color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;

  .logo {
    width: 132px;
    height: 26px;

    img {
      width: 100%;
      height: 100%;
    }
  }

  .add {
    img {
      &:first-child {
        margin-right: 17px;
      }
    }
  }
}

.title {
  width: 100%;
  height: 52px;
  background-color: #4a92e3;
  color: #fff;
  font-size: 18px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.notice {
  width: 100%;
  height: 42px;
  background-color: #fefbeb;
  line-height: 42px;
  padding-left: 15px;
  font-size: 16px;
}

ul {
  background-color: #fff;

  li {
    width: 100%;
    height: 54px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-left: 20px;
    border-bottom: 1px solid #ececec;

    .left {
      font-size: 20px;
    }

    .right {
      // margin-right: 5px;
      font-size: 20px;
      color: #ccc;
      input {
        height: 54px;
        // background-color: pink;
        font-size: 20px;

        &::placeholder {
          color: #ccc;
        }
      }
    }
  }
}

.js {
  width: 100%;
  height: auto;
  font-size: 16px;
  padding: 20px 16px;
  color: #8f8f8f;
}

.search {
  width: 100%;
  height: 57px;
  padding: 0 15px;

  button {
    width: 345px;
    height: 57px;
    background-color: #4a92df;
    border: unset;
    font-size: 20px;
    color: #fff;
    cursor: pointer;
  }
}
.footer {
  background-color: rgb(40, 40, 40);
  color: rgb(117, 117, 117);
  margin-top: 50px;
  font-size: 12px;
  padding: 20px 40px;
  p {
    margin-top: 5px;
  }
}
</style>
