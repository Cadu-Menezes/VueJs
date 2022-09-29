<template>
<div class="Principal">
  
  <div class="BackgroundImage">
    <div >
      <q-parallax src="https://cdn.quasar.dev/img/parallax2.jpg">
        <h1 class="text-white">Gamaria Advogados</h1>
      </q-parallax>
    </div>
  </div>

  <h1 id="TituloAtuacao">Áreas de atuação</h1>

  <div class="q-pa-md">
    <div class="q-gutter-y-md" >
      <q-tabs v-model="tab" dense class="bg-grey-2 text-teal">
        <q-tab name="mails" icon="mail" label="Mails"></q-tab>
        <q-tab name="alarms" icon="alarm" label="Alarms" />
        <q-tab name="movies" icon="movie" label="Movies" />
      </q-tabs>
    </div>
  </div>




</div>
</template>


<script>
  import { defineComponent } from 'vue'
  import { ref } from 'vue'

  export default defineComponent({
    name: 'IndexPage',
   


    setup() {
    return {
      tab: ref(''),
    }
  }
  
  })
</script>




<style scoped>
  .Principal{
    height: 100%;
  }

  .BackgroundImage{
      display: block;
      width: 100vw;
      height: 100vh;
      padding: 0;
      text-align: center;
      color: white;
      background: url(https://cdn.quasar.dev/img/parallax2.jpg) no-repeat bottom center scroll;
      background-color: black;
      -webkit-background-size: contain;
      -moz-background-size: contain;
      background-size: contain;
      -o-background-size: contain;
  }

  .q-pa-md{
    width: 100%;
  }

  #TituloAtuacao{
      
      display: flex;
      text-align: center;
      margin-left: 300px;
  }

</style>
