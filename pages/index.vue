<template>
  <v-app>
    <v-app-bar
      app
      color="#f6f6f6"
      flat
      light
      outlined
    >
      <v-app-bar-title>
        <span class="d-flex align-end">
          <span style="height: 32px;width: 32px;line-height: 32px;margin-right: 2px;">
            <img src="../static/icon.png">
          </span>
          ReadyRun
        </span>
      </v-app-bar-title>
    </v-app-bar>
    <v-main>
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
            Windows 版下载
          </v-btn>
        </div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>

export default {}
</script>

<style module scoped>
.container {
  max-width: 960px;
  margin: 0;
  padding: 0;
  margin: 0 auto;
}

.page {
  margin: 0 auto;
  padding-top: 72px;
}

.image {
  height: 320px;
  background-image: url("../static/download-bg.jpg");
  background-size: cover;
  background-position: 50%;
}
</style>
