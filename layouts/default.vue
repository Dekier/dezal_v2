<template>
  <div>
    <NavBar />
    <slot />
  </div>
</template>

<script>
export default {
  name: "LayoutDefault",
};
</script>
<style lang="scss" scoped>
@import "default";
</style>
