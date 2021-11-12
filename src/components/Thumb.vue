<template>
  <div class="thumb col-2">
      <img :src="albumImage" alt="">
      <h5>{{typeAlbum}}</h5>
  </div>
</template>

<script>
export default {
  props: {
    albumImage: String,
    typeAlbum: String
  }
}
</script>

<style>
</style>
