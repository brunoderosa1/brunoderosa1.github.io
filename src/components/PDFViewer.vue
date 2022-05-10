<template>
<div class="container">
    <hr>
    <iframe class="reader" src="https://www.soundczech.cz/temp/lorem-ipsum.pdf" frameborder="0"></iframe>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
  display: block;
  position:fixed;
  bottom: 5%;
  right: 5%;
  left: 5%;
}
.reader {
    width:100%;
    height:30rem;
}
</style>
