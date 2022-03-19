<template>
  <div class="logo m-v-14 position-relative">
    <img
      src="https://www.instagram.com/static/images/web/mobile_nav_type_logo.png/735145cfe0a4.png"
      alt="Logo"
      class="cur-p"
      @click="goHome"
    />
  </div>
</template>

<script>
export default {
  name: "Logo",
  methods: {
    goHome() {},
  },
};
</script>

<style lang="scss">
.logo {
  top: 4px;
}
</style>