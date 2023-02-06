<template>
  <div class="CenterPanel__main-container">
    <Post v-for="n in 10" :key="n"></Post>
  </div>
</template>
<style lang="scss" scoped>
@import "CenterPanel";
</style>
