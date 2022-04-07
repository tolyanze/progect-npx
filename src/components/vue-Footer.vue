<template>
  <footer>
    <div class="container">
      <ul class="navbar-list">
        <li class="navbar-item" v-for="link in links" :key="link"><a :href="link.url" class="navbar-link">{{link.alias}}</a></li>
      </ul>
    </div>
  </footer>
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