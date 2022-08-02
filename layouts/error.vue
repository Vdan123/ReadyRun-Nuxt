<template>
  <v-container style="padding: 120px 40px">
    <h1>
      是否找不到方向？
    </h1>
    <div :class="$style.content">
      陌生人，你看起来很迷茫。你知道，在迷茫的时候，什么能帮上忙吗？是一碗热乎乎的面条。
    </div>
    <v-btn
      dark
      style="border-radius: 28px"
      @click="navigateHome"
    >
      返回首页
    </v-btn>
  </v-container>
</template>

<script>
export default {
  props: {
    error: {
      type: Object,
      default: () => ({})
    }
  },
  methods: {
    navigateHome() {
      return this.$router.push('/')
    }
  }
}
</script>

<style module scoped>
.content {
  margin: 20px 0;
  font-size: 20px;
  color: rgb(0, 0, 0);
}
</style>
