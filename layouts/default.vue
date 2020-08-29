<template>
  <div>
    <Header />
    <main class="main-content">
      <nuxt/>
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header/Header'
export default {
  components: {
    Header
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  /* color: brown; */
}
body {
  font-family: sans-serif;
  /* height: 100vh; */
  margin: 0;
  background:
      linear-gradient(217deg, rgba(0,0,255,.8), rgba(255,0,0,0) 70.71%),
      linear-gradient(127deg, rgba(0,255,0,.8), rgba(0,255,0,0) 70.71%),
      linear-gradient(336deg, white, rgba(0,0,255,0) 70.71%);
  /* background-repeat: no-repeat; */
  /* background-size: cover; */
}
.main-content {
  margin-top: 6rem;
}
</style>
