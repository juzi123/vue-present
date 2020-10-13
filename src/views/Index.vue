<template>
  <div>
    <Header></Header>
    <div class="main-layout">
      <LeftMenu></LeftMenu>
      <Content></Content>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import Header from "@/components/layouts/Header";
import LeftMenu from "@/components/layouts/LeftMenu";
import Content from "@/components/layouts/Content";
export default {
  components: { LeftMenu, Header, Content }
};
</script>

<style lang="scss" scoped>
.main-layout {
  display: flex;
  flex-direction: row;
}
</style>
