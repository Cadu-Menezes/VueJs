<template>
  <div class="Principal">
    <div class="BackgroundImage">
      <div>
        <q-parallax src="https://cdn.quasar.dev/img/parallax2.jpg">
          <h1 class="text-white">Gamaria Advogados</h1>
        </q-parallax>
      </div>
    </div>

    <div class="Titulos">
      <h1 class="text-black">Áreas de atuação</h1>
    </div>

    <div>
      <q-splitter v-model="splitterModel" style="height: 250px">
        <template v-slot:before>
          <q-tabs v-model="tab" vertical class="text-teal">
            <q-tab name="mails" icon="mail" label="Mails" />
            <q-tab name="alarms" icon="alarm" label="Alarms" />
            <q-tab name="movies" icon="movie" label="Movies" />
          </q-tabs>
        </template>

        <template v-slot:after>
          <q-tab-panels
            v-model="tab"
            animated
            swipeable
            vertical
            transition-prev="jump-up"
            transition-next="jump-up"
          >
            <q-tab-panel name="mails">
              <div class="text-h4 q-mb-md">Mails</div>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
            </q-tab-panel>

            <q-tab-panel name="alarms">
              <div class="text-h4 q-mb-md">Alarms</div>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
            </q-tab-panel>

            <q-tab-panel name="movies">
              <div class="text-h4 q-mb-md">Movies</div>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quis
                praesentium cumque magnam odio iure quidem, quod illum numquam
                possimus obcaecati commodi minima assumenda consectetur culpa
                fuga nulla ullam. In, libero.
              </p>
            </q-tab-panel>
          </q-tab-panels>
        </template>
      </q-splitter>
    </div>
  </div>
</template>


<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "IndexPage",

  setup() {
    return {
      tab: ref("Mails"),
    };
  },
});
</script>




<style scoped>
.Principal {
  height: 100%;
}

.BackgroundImage {
  display: block;
  width: 100vw;
  height: 100vh;
  padding: 0;
  text-align: center;
  color: white;
  background: url(https://cdn.quasar.dev/img/parallax2.jpg) no-repeat bottom
    center scroll;
  background-color: black;
  -webkit-background-size: contain;
  -moz-background-size: contain;
  background-size: contain;
  -o-background-size: contain;
}

.q-pa-md {
  width: 100%;
}

.Titulos {
  text-align: center;
}
</style>
