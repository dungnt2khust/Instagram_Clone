<template>
  <div
    class="header w-100 d-flex p-h-20 flex-row justify-content-between align-items-center"
  >
    <Logo />
    <Search class="d-none d-sm-none d-md-block" />
    <Controls />
  </div>
</template>

<script>
import Logo from "../components/Logo/Logo";
import Search from "../components/Search/Search";
import Controls from "../components/Controls/Controls";
export default {
  name: "Header",
  components: {
    Logo,
    Search,
    Controls,
  },
};
</script>

<style lang="scss">
.header {
  width: 100%;
  max-width: 1000px;
}
</style>