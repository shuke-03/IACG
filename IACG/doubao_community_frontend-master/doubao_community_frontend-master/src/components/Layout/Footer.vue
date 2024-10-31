<template>
  <footer class="footer has-text-grey-light has-background-grey-darker">
    <div class="container">
      <div class="">
        <span>此生无悔入二次元</span>

        <span style="float: right">
          <router-link :to="{path:'/admin/login'}">
           
          </router-link>
          |
          <a href="/?lang=zh_CN">聂佳豪</a> |
          <a href="/?lang=zh_CN">李裕安</a> |
          <a href="/?lang=en_US">黄嘉程</a>
        </span>
      </div>

      <div>
        <span>{{ title }} ALL RIGHTS RESERVED</span>
        <div style="float: right">
          <template>
            <b-taglist attached>
              <b-tag type="is-dark" size="is-normal">Design</b-tag>
              <b-tag type="is-info" size="is-normal">{{ author }}</b-tag>
            </b-taglist>
          </template>
        </div>
      </div>
    </div>
    <back-top></back-top>
  </footer>
</template>

<script>
import BackTop from "@/components/Backtop/BackTop";

export default {
  name: "Footer",
  components: {
    BackTop
  },
  data() {
    return {
      title: "© " + new Date().getFullYear() + ' 二次元社区',
      author: '二次元社区',
    };
  },
};
</script>

<style scoped>

footer {
  margin-top: 120px;
  height: 150px;
}
footer a{
  color: #bfbfbf;
}

</style>