<template>
  <v-sheet>
    <h1 :class="$style.title">
      ReadyRun for Windows
    </h1>
    <div :class="$style.desc" class="mt-8 mb-4">
      一次冒险之旅在等着你哟。在我们的桌面APP上，开始高效的工作吧。
    </div>
    <v-btn
      class="mx-auto mt-2"
      color="#23272a"
      dark
      href="http://10.255.128.149/download/flavor/ReadyRun/1.1.5/windows_64/ReadyRun.Setup.1.1.5.exe"
      style="border-radius: 28px;"
      x-large
    >
      <v-icon class="mr-2">
        mdi-download
      </v-icon>
      <span class="text-capitalize">
        Windows_1.1.5 版下载
      </span>
    </v-btn>
  </v-sheet>
</template>

<script>
export default {
  name: 'Downloads'
}
</script>

<style module scoped>
.title {
  font-size: clamp(24px, 5vw, 44px);
}

.desc {
  font-size: clamp(16px, 2vw, 20px);
}
</style>
