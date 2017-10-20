<template>
<div>
   <header>
      <span>SGS商场</span>
      <ul>
        <li>登录</li>
        <li>注册</li>
        <li><nuxt-link :to="{name:'index-personalCenter'}">个人中心</nuxt-link></li>
        <li><nuxt-link :to="{name:'index-myOrder'}">我的订单</nuxt-link></li>
        <li><nuxt-link :to="{name:'index-shoppingCart'}">购物车</nuxt-link></li>
      </ul>
    </header>
     <section class="container">
       <nuxt-child></nuxt-child>
     </section>
    <footer>222</footer>
</div>
 
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
