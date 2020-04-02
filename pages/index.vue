<template>
  <div class="container">
    <div>
      <h1 class="title">
      </h1>
      <h2 class="subtitle">
      </h2>
      <div class="main_section">
        <Main />
        <div class="links">
          <nuxt-link to="/intro" class="link">입관안내서</nuxt-link>
        </div>
      </div>
      
      
      
    </div>
  </div>
</template>

<script>
import Main from '~/components/Main.vue'

export default {
  components: {
    Main
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
}

.subtitle {
}

.main_section {
  position: relative;
  height: 100vh;
}

.links {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  margin-bottom: 100px;
}

.link {
  color: #fff;
  text-decoration: none;
  display: inline-block;
  padding: 10px 15px;
  font-size: 18px;
  border: 1px solid #fff;
  border-radius: 10px;
}

.link:hover{
  background-color: #5d5c5c;
}
</style>
