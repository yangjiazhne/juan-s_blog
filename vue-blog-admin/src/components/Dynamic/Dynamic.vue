<template>
  <div class="dynamic-box">
    <h3>动态</h3>
    <div class="no-activity" v-if="isEmpty">
      <svg-icon icon-class="empty" class-name="empty" />
    </div>
    <div class="contribution-in-date" v-if="!isEmpty">
      <div class="header">
        <div class="timeline-on date">06.16</div>
      </div>
      <div class="content">
        <!--   每一种动态类型，共有三种：文章提交commit、文章修改edit、文章删除remove     -->
        <div class="contributions">
          <div class="header">
            <!--     三种图标：commit、edit、remove       -->
            <div class="timeline-on icon">
              <svg-icon icon-class="commit" class-name="commit" />
            </div>
            <div class="summary">新增了2篇博客</div>
          </div>
          <ul class="list">
            <li v-for="index of 2" :key="index">
              <a href="#">￥含含￥</a>
              <span>软件工程博客编辑</span>
            </li>
          </ul>
        </div>

        <div class="contributions">
          <div class="header">
            <!--     三种图标：commit、edit、remove       -->
            <div class="timeline-on icon">
              <svg-icon icon-class="edit" class-name="edit" />
            </div>
            <div class="summary">修改了2篇博客</div>
          </div>
          <ul class="list">
            <li>
              <a href="#">￥烟烟￥</a>
              <span>1次修改</span>
            </li>
            <li>
              <a href="#">￥思思￥</a>
              <span>2次修改</span>
            </li>
          </ul>
        </div>

        <div class="contributions">
          <div class="header">
            <!--     三种图标：commit、edit、remove       -->
            <div class="timeline-on icon">
              <svg-icon icon-class="remove" class-name="remove" />
            </div>
            <div class="summary">删除了1篇博客</div>
          </div>
          <ul class="list">
            <li>
              <a href="#">￥洋洋￥</a>
              <span>java爬虫</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Dynamic",
  props: {},
  components: {},
  data() {
    return {
      isEmpty: false,
    };
  },
  methods: {},
  computed: {},
  watch: {},
  mounted() {},
};
</script>

<style scoped lang="scss">
@import "Dynamic";
</style>
