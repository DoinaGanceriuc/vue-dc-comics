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

<style lang="scss">
.thumb {
  height: 200px;
  padding: 1rem;
  img {
    height: 100%;
    object-fit: cover;
    object-position: top;
    width: 100%;
  }
  h5 {
    color: #fff;
    padding-top: 1rem;
  }
}
</style>
