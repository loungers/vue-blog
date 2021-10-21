<template>
  <div class="main">
    <div class="top">
      <div class="logo">
        <div class="title">{{ webTitle }}</div>
      </div>
      <div class="menu">
        <ul class="menuBox">
          <li class="menuList" v-for="list in menuList" :key="list.name1">
            <div class="listTitle">{{ list.name1 }}</div>
          </li>
        </ul>
      </div>
    </div>
    <div class="left"></div>
    <div class="center"></div>
    <div class="right"></div>
    <div class="buttom"></div>
  </div>
</template>

<script>
export default {
  name: "Index",
  props: {},
  data: function() {
    return {
      webTitle: "Loungersの自留地",
      menuList: [
        { name1: "第一" },
        { name1: "第二", name2: "第二的第二" },
        { name1: "第三" },
        { name1: "第四"},
        { name1: "第五"}
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main {
  min-height: calc(100vh - 1.5em);
  // height: 100vh;
  // width: auto;
  background: url("../assets/images/background.jpg") no-repeat center fixed;
  background-size: 100%;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  padding-top: 1.5em;

  .top {
    margin: 0 auto;
    width: 98%;
    height: 4em;
    border-radius: 15px;
    background: #d0d6ee; /* 注释后变透明 */
    box-shadow: 18px 18px 35px #f0eff7, -18px -18px 35px #ffffff;

    .logo {
      float: left;

      .title {
        padding: 1.3em 0 0 2em;
        // height: 2em;
        float: left;
      }
    }

    .menu {
      margin-left: 55vw;

      .menuBox {
        /* 去除列表点 */
        margin: 0;
        padding: 0;
        list-style-type: none;
        /* 靠右 */

        .menuList {
          /*并列排放*/
          display: inline;

          .listTitle {
            text-align: center;
            height: 4em;
            line-height: 4em;
            width: 6em;
            // background: #d0d6ee;
            float: left;
          }
        }
      }
    }
  }
}
</style>
