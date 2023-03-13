<template>
  <div class="video-container">
    <video autoplay muted loop>
      <source src="../assets/store.mp4" type="video/mp4">
  </video>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.video-container{
  width: 100%;
}
video{
  width: 100%;
  box-shadow: inset 0px 0px 64px rgba(0,0,0,1);
}

</style>
