<template>
  <el-container id="one">
    <el-aside :class="{'fold':isCollapse,'unfold':!isCollapse}">
      <div class="left_top">
        <div class="title">
          <span v-show="!isCollapse">校园跑腿</span>
        </div>
        <div class="select">
          <el-menu :default-active="this.$route.path" :router="true" :unique-opened="true" class="el-menu-vertical-demo" 
          @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff"  active-text-color="#ffd04b" :collapse="isCollapse">
<<<<<<< HEAD
=======
<<<<<<< HEAD
>>>>>>> b65b59ab0d5449b2ee7bc59db5a5c251f9bad8a4
            <el-menu-item index="/firstPage/mainPage">
              <i class="el-icon-s-home"></i>
              <span slot="title">首页</span>
            </el-menu-item>
            <el-menu-item index="/firstPage/buy">
              <i class="el-icon-s-shop"></i>
              <span slot="title">代买商品</span>
            </el-menu-item>
            <el-menu-item index="/firstPage/post">
              <i class="el-icon-goods"></i>
              <span slot="title">代送物品</span>
            </el-menu-item>
            <el-menu-item index="/firstPage/get">
              <i class="el-icon-s-claim"></i>
              <span slot="title">代取物品</span>
            </el-menu-item>
            <el-menu-item index="/firstPage/sort">
              <i class="el-icon-s-data"></i>
              <span slot="title">代排队</span>
            </el-menu-item>
            <el-submenu index="3">
              <template slot="title">
                <i class="el-icon-user-solid"></i>
                <span>个人中心</span>
              </template>
              <el-menu-item-group>
                <el-menu-item index="/firstPage/myBuy">发布的代买信息</el-menu-item>
                <el-menu-item index="/firstPage/myPost">发布的代送信息</el-menu-item>
                <el-menu-item index="/firstPage/myGet">发布的代取信息</el-menu-item>
                <el-menu-item index="/firstPage/mySort">发布的代排队信息</el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-submenu index="4">
              <template slot="title">
                <i class="el-icon-warning-outline"></i>
                <span>跑腿审核</span>
              </template>
              <el-menu-item-group>
                <el-menu-item index="/firstPage/checkBuy">代买信息</el-menu-item>
                <el-menu-item index="/firstPage/checkPost">代送信息</el-menu-item>
                <el-menu-item index="/firstPage/checkGet">代取信息</el-menu-item>
                <el-menu-item index="/firstPage/checkSort">代排队信息</el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-menu-item index="/firstPage/userManager">
              <i class="el-icon-menu"></i>
              <span slot="title">用户管理</span>
            </el-menu-item>
<<<<<<< HEAD
=======
=======
                <el-menu-item index="/firstPage/mainPage">
                  <i class="el-icon-s-home"></i>
                  <span slot="title">首页</span>
                </el-menu-item>
                <el-menu-item index="/firstPage/buy">
                  <i class="el-icon-s-shop"></i>
                  <span slot="title">代买商品</span>
                </el-menu-item>
                <el-menu-item index="/firstPage/post">
                  <i class="el-icon-goods"></i>
                  <span slot="title">代送物品</span>
                </el-menu-item>
            
                <el-menu-item index="/firstPage/get">
                  <i class="el-icon-s-claim"></i>
                  <span slot="title">代取物品</span>
                </el-menu-item>
                <el-menu-item index="/firstPage/sort">
                  <i class="el-icon-s-data"></i>
                  <span slot="title">代排队</span>
                </el-menu-item>
                <el-submenu index="3">
                  <template slot="title">
                    <i class="el-icon-user-solid"></i>
                    <span>个人中心</span>
                  </template>
                  <el-menu-item-group>
                    <el-menu-item index="/firstPage/myBuy">发布的代买信息</el-menu-item>
                    <el-menu-item index="/firstPage/myPost">发布的代送信息</el-menu-item>
                    <el-menu-item index="/firstPage/myGet">发布的代取信息</el-menu-item>
                    <el-menu-item index="/firstPage/mySort">发布的代排队信息</el-menu-item>
                  </el-menu-item-group>
                </el-submenu>
>>>>>>> 5db1772f9706f53ae3dbc727bf5a2b2e5f92e27a
>>>>>>> b65b59ab0d5449b2ee7bc59db5a5c251f9bad8a4
          </el-menu>
        </div>
      </div>
      <div class='goBack'>
        <i class="el-icon-arrow-left"></i>
      </div>
    </el-aside>
    <el-container>
      <el-header>
        <div class="top_left">
          <i class="el-icon-s-unfold" v-show='isCollapse' @click="unFold"></i>
          <i class="el-icon-s-fold" v-show='!isCollapse' @click="fold"></i>
          <span class="firstPage">{{title}}</span>
        </div>
        <el-row>
          <el-menu class="el-menu-demo" mode="horizontal" @select="handleSelect"  :default-active="this.$route.path" :router="true" :unique-opened="true" >
            <el-submenu index="1" id="other">
              <template slot="title">
                <div class="block"><el-avatar :size="50" :src="$store.state.avatar" fit='contain'></el-avatar></div>
              </template>
              <el-menu-item index="/firstPage/userInfo" v-if="id">
                <i class="el-icon-user"></i>个人信息</el-menu-item>
              <el-menu-item index="/firstPage/message" v-if="id">
<<<<<<< HEAD
                <i class="el-icon-bell"></i>消息提醒</el-menu-item>
=======
<<<<<<< HEAD
                <i class="el-icon-bell"></i>消息提醒</el-menu-item>
=======
                <i class="el-icon-message"></i>消息提醒</el-menu-item>
>>>>>>> 5db1772f9706f53ae3dbc727bf5a2b2e5f92e27a
>>>>>>> b65b59ab0d5449b2ee7bc59db5a5c251f9bad8a4
              <el-menu-item index="/firstPage/setting" v-if="id">
                <i class="el-icon-setting"></i>设置</el-menu-item>
              <el-menu-item index="/firstPage/quit" @click="quit">
                <i class="el-icon-switch-button"></i>退出</el-menu-item>
            </el-submenu>
          </el-menu>
          <el-link type="primary" @click="toLogin" v-show='!id'>登录</el-link>
          <el-link type="info" @click="toRegister" v-show='!id'>注册</el-link>
        </el-row>
      </el-header>
      <el-main>
        <router-view />
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
export default {
  name:'firstPage',
  data() {
    return {
      id:'', //用户id
      title:'',
      isCollapse: false, //是否折叠
      activeIndex: "",
      // avatar: "https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png", //头像
    };
  },
  watch: {
    $route: "watchRoute"
  },
  created(){
    var id = JSON.parse(sessionStorage.getItem('id')) //用户id
    // var src = JSON.parse(sessionStorage.getItem('avatar')) //用户id
    if(id){
      this.id = id
    }
    console.log(this.id)
      //  console.log(src)
  },
  mounted() {
    this.watchRoute();
  },
   methods: {
    watchRoute() {
      var path = this.$route.path
      console.log(path);
      if(path == '/firstPage/buy'){
        this.title = '代买商品'
      }else if(path == '/firstPage/post'){
        this.title = '代送物品'
      }else if(path == '/firstPage/get'){
        this.title = '代取物品'
      }else if(path == '/firstPage/sort'){
        this.title = '代排队'
      }else if(path == '/firstPage/myBuy'){
        this.title = '个人中心 / 发布的代买信息'
      }else if(path == '/firstPage/myPost'){
        this.title = '个人中心 / 发布的代送信息'
      }else if(path == '/firstPage/myGet'){
        this.title = '个人中心 / 发布的代取信息'
      }else if(path == '/firstPage/mySort'){
        this.title = '个人中心 / 发布的代排队信息'
      }else if(path == '/firstPage/mainPage'){
        this.title = '首页'
      }else if(path == '/firstPage/userInfo'){
        this.title = '个人信息'
      }else if(path == '/firstPage/setting'){
        this.title = '设置'
      }else if(path == '/firstPage/message'){
        this.title = '消息提醒'
<<<<<<< HEAD
=======
<<<<<<< HEAD
>>>>>>> b65b59ab0d5449b2ee7bc59db5a5c251f9bad8a4
      }else if(path == '/firstPage/checkBuy'){
        this.title = '跑腿审核 / 代买信息'
      }else if(path == '/firstPage/checkPost'){
        this.title = '跑腿审核 / 代送信息'
      }else if(path == '/firstPage/checkGet'){
        this.title = '跑腿审核 / 代取信息'
      }else if(path == '/firstPage/checkSort'){
        this.title = '跑腿审核 / 代排队信息'
      }else if(path == '/firstPage/userManager'){
        this.title = '用户管理'
<<<<<<< HEAD
=======
=======
>>>>>>> 5db1772f9706f53ae3dbc727bf5a2b2e5f92e27a
>>>>>>> b65b59ab0d5449b2ee7bc59db5a5c251f9bad8a4
      }
    },
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    },
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
    // 登录
    toLogin:function(){
      this.$router.push({path:'/index/login/passwordLogin'})
    },
    // 注册
    toRegister:function(){
      this.$router.push({path:'/index/register'})
    },
    unFold:function(){
      this.isCollapse = false
    },
    fold:function(){
      this.isCollapse = true
    },
    quit:function(){
      this.$router.push({path:'/index/login'})
    }
  }
}
</script>

<style scoped>
  .fold{
    width:64px !important;
  }
  .unfold{
    width:200px !important;
  }
  .top_left{
    display:flex;
    flex-direction:row;
    align-items: center;
  }
  .el-icon-s-unfold,.el-icon-s-fold{
    font-size:40px
  }
  .el-menu-vertical-demo:not(.el-menu--collapse) {
    width: 200px;
    min-height: 400px;
  }
  a{
    text-decoration: none;
    color:#eee;
  }
 .el-header {
    background-color: #545c64;
    color: #333;
    text-align: center;
    line-height: 60px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  
  .el-aside {
    background-color:#545c64;
    color: #333;
    text-align: center;
    width:100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    box-sizing: border-box;
  }
  .left_top{
    width:100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    /* text-align: center; */
    display: flex;
    flex-direction: column;
  }
  #one{
    width:100%;
    height:100vh;
  }

.title{
  width:100%;
  height:60px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  background-color: rgb(31, 39, 54);
  color:white;
}
.title span{
  font-size: 20px;
  letter-spacing: 2px;
  font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;
}
.select{
  width:100%;
}
.one,.two,.three,.four{
  width:50%;
  height:60px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  color:#eee;
}
.goBack{
  width:100%;
  background-color: rgb(31, 39, 54);
  height:40px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  color:white;
}
.right_top{
  width: 100%;
  height:100px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.topTitle{
  height:50%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  font-size: 18px;
  font-weight: bold;
}
.el-col-12{
  width:100%;
}
/* li{
  width:200px !important;
} */
/* 头像 登录 注册 */
.el-row{
  display: flex;
  flex-direction: row;
  align-items: center;
}
.block{
  width:50%;
  height:50px
}
/* 注册 */
.el-link.el-link--info{
  width:50px
}
/* 登录 */
.el-link.el-link--primary{
  width:50px
}
.el-menu{
  border-right:none
}
/* 首页 */
.firstPage{
  margin-left:10px;
  color:white;
  font-size: 18px;
}
>>>#other .el-submenu__title i{
  display: none;
}
>>>.el-menu--horizontal>.el-submenu{
  background-color: rgb(84, 92, 100);
}
>>>.el-menu--horizontal>.el-submenu.is-active .el-submenu__title{
  border-bottom: none;
}
>>>.el-menu--horizontal>.el-submenu:hover{
  background-color: rgb(84, 92, 100);
}
</style>
