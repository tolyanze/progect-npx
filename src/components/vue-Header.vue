<template>
  <header>
    <div class="navbar">
      <div class="container">
        <div class="navbar-content">
          <a href="/" class="navbar-logo">logo</a>
          <ul class="navbar-list">
            <li class="navbar-item" v-for="link in links" :key="link"><a :href="link.url" class="navbar-link">{{link.alias}}</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  props:{
    links:{
      type: Array,
      required: true
    }
  }

}
</script>

<style>

</style>