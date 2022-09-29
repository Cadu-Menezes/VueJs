<template>
  <q-layout view="lHh Lpr lFf">
    
    <q-header elevated class="topo">
      <q-toolbar>
    
        <q-toolbar-title id="Titulo">
          Gamaria Adv 
        </q-toolbar-title>

        <q-btn :ripple="false" color="black" label="No ripple" no-caps class="Btn-Menu"/>
        <q-btn :ripple="{ color: 'yellow' }" color="black" label="Yellow ripple" no-caps class="Btn-Menu"/>
        <q-btn :ripple="{ center: true }" color="black" label="Center ripple" no-caps class="Btn-Menu"/>

      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
  
</template>

<script>
import { defineComponent, ref } from 'vue'


export default defineComponent({
  name: 'MainLayout',


  setup () {
    const leftDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>

sty/<style lang="scss">
.Btn-Menu{
margin-left: 20px;
}

.topo{
  background-color: #F0FFFF;
}

#Titulo{
  color: black;
}
</style>
