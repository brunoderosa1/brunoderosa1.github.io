<template>
  <div class="app">
    <div class="cage">
      <h1 class="title">Visualizador de PDF</h1>
    <p class="paragraph-1">Al presionar el boton, se abrira una ventana superpuesta donde se visualizara un archivo PDF utilizando un elemento iframe</p>
    <button class="btn1" @click="iframeViewer" v-if="!iframeIsVisible">Presione para ver</button>
    <button class="btn2" @click="iframeViewer" v-else>Presione para ocultar</button>
    </div>
    <PDFViewer v-if='iframeIsVisible' />
  </div>
</template>

<script>
import PDFViewer from '@/components/PDFViewer.vue'

export default {
  components: { PDFViewer },
  data () {
    return {
      iframeIsVisible: false
    }
  },
  methods: {
    iframeViewer () {
      this.iframeIsVisible = !this.iframeIsVisible
    }
  }
}
</script>

<style scoped>
.cage {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.title {
  font-family: Helvetica, sans-serif;
  color:rgb(29, 152, 83);
  text-align: center;
  font-weight: 600;
  text-shadow: 1mm;
}
.paragraph-1 {
  font-family: Arial, Helvetica, sans-serif;
  color:rgb(29, 152, 83);
  text-align: center;
}
.btn1 {
  width: 300px;
  border-radius: 0.5rem 0.5rem 0.5rem 0.5rem;
}
.btn1:hover {
  color:turquoise;
  animation: loop 3s infinite;
  border-radius: 0.5rem 0.5rem 0.5rem 0.5rem;
}
.btn2 {
  width: 300px;
  border-radius: 0.5rem 0.5rem 0.5rem 0.5rem;
}

@keyframes loop {
  0% { background-color: orange; }
  25% { background-color: orangered; }
  50% { background-color: orange; }
  75% {background-color: orangered;}
  100%{ background-color: orange;}
}
</style>
