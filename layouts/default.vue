<template>
  <v-app id="app">
    <v-app-bar
      app
      color="#f6f6f6"
      flat
      light
      outlined
    >
      <v-app-bar-title>
        <span class="d-flex align-end" style="cursor: pointer" @click="navigateHome">
          <span style="height: 32px;width: 32px;line-height: 32px;margin-right: 2px;">
            <img src="../static/icon.png">
          </span>
          ReadyRun
        </span>
      </v-app-bar-title>
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  methods: {
    navigateHome() {
      console.log('fooo')
      this.$router.push('/')
    }
  }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro',
  -apple-system,
  BlinkMacSystemFont,
  'Segoe UI',
  Roboto,
  'Helvetica Neue',
  Arial,
  sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
