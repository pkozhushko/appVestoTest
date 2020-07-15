<template>
  <div class="header__wrapper">
    <div class="logo__wrapper">
      <div class="logo"></div>
      <div class="line"></div>
      <div class="additional-text"></div>
    </div>
    <div class="alter-logo__wrapper">
      <div class="alter-additional-text"></div>
      <div class="line"></div>
      <div class="alter-logo"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header__wrapper {
  width: 100%;
  background: rgb(0, 0, 0);
  height: 60px;
  position: absolute;
  top: 0px;
  display: flex;
  justify-content: space-between;
  color: #fff;
  padding: 0 50px;
  box-sizing: border-box;
}
.logo__wrapper,
.alter-logo__wrapper {
  display: flex;
}
.logo {
  width: 100px;
  height: 100%;
  background: transparent url("../assets/SparkLogo.png") center no-repeat;
}
.line {
  width: 1px;
  height: 39px;
  margin: 9px 15px;
  background: #8d8d8d;
}
.additional-text {
  width: 50px;
  height: 100%;
  background: transparent url("../assets/LiveEvents.png") center no-repeat;
}

.alter-logo {
  width: 100px;
  height: 100%;
  padding-right: 15px;
  background: transparent url("../assets/alter-logo.png") center no-repeat;
  position: relative;
}
.alter-additional-text {
  width: 50px;
  height: 100%;
  background: transparent url("../assets/alter-text.png") center no-repeat;
}
</style>
