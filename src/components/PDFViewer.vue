<template>
<div class="container">
    <hr>
    <iframe class="reader" src="https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf" frameborder="0"></iframe>
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
