<template>
  <div class="bg-gray-950 flex justify-center items-center h-screen ">
    <div class="flex flex-row bg-div-p rounded-md ">
      <div>
        <NomeFoto/>
        <DadosLeo/>
      </div>
      <div class="text-orange"> Resume</div>
    </div>
  </div>
</template>


<script>
import NomeFoto from './components/NomeFoto.vue'
import DadosLeo from './components/DadosLeo.vue'

export default {
  name: 'App',
  components: {
    NomeFoto,
    DadosLeo
  }
}
</script>

<style>
.bg-fundo {
  background-color: #313E50;
}
.text-orange {
  color: #ffc107;
}
.bg-div-p{
  background-color: #24242f;
}
.bg-div-foto{
  background-color: #26262e;
}
.bg-div{
  background-color: #2b2b35;
}

</style>