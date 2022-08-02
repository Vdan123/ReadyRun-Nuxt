<template>
  <v-container :class="$style.container" fluid>
    <div :class="$style.page">
      <h2>
        Download
      </h2>
      <div :class="$style.image" />
    </div>

    <div class="d-flex my-4">
      <v-btn
        class="mx-auto"
        color="#23272a"
        dark
        large
        style="border-radius: 28px;"
      >
        <v-icon class="mr-2">
          mdi-download
        </v-icon>
        <span class="text-capitalize">
          Windows 版下载
        </span>
      </v-btn>
    </div>
  </v-container>
</template>

<script>
export default {
  name: 'Downloads'
}
</script>

<style module scoped>
.container {
  max-width: 960px;
  padding: 0;
  margin: 0 auto;
}

.page {
  margin: 0 auto;
  padding-top: 72px;
}

.image {
  height: 320px;
  background-image: url("../../static/download-bg.jpg");
  background-size: cover;
  background-position: 50%;
}
</style>
