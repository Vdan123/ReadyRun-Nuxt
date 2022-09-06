<template>
  <v-container :class="$style.container" fluid>
    <v-row :class="$style.page">
      <v-col>
        <v-slide-x-reverse-transition>
          <div v-show="show" :class="$style.image" />
        </v-slide-x-reverse-transition>
      </v-col>
      <v-col>
        <v-slide-y-reverse-transition>
          <Downloads v-show="show" />
        </v-slide-y-reverse-transition>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Downloads from '../components/Downloads'

export default {
  name: 'App',
  components: {
    Downloads
  },
  data() {
    return {
      show: false
    }
  },
  mounted() {
    setTimeout(() => {
      this.show = true
    }, 400)
  }
}
</script>

<style module scoped>
.container {
  max-width: 1180px;
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
