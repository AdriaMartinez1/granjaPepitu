<template>
  <ion-header>
    <ion-toolbar>
      <ion-title>La Granja d'en Pepitu</ion-title>
    </ion-toolbar>
  </ion-header>

  <ion-content color="light" style="overflow-y: auto;">
    <ion-list :inset="true">
      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/ruc.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>RUC</h2>
          <p>Un animal pacient amb grans orelles que camina al seu ritme pel camp</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/ruc.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/xai.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>XAI</h2>
          <p>Petit i saltarí, el xai porta la innocència de la primavera</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/xai.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/anec.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>ÀNEC</h2>
          <p>Amb el seu quac característic, l’ànec gaudeix de l’aigua i l’aire</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/anec.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/porc.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>PORC</h2>
          <p>Alegre i fangós, el porc gaudeix de les petites coses de la vida</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/porc.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/cavall.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>CAVALL</h2>
          <p>Imponent i elegant, el cavall corre lliurement pel camp</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/cavall.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/ovella.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>OVELLA</h2>
          <p>Tranquil·la i suau, l’ovella pastura en harmonia amb la natura</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/ovella.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/vaca.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>VACA</h2>
          <p>Serpentejant pel prat, la vaca rumia lentament i amb calma</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/vaca.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/gallina.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>GALLINA</h2>
          <p>Amb el seu cant matutí, la gallina comença el dia a la granja</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/gallina.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/cabra.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>CABRA</h2>
          <p>Curiosa i enèrgica, la cabra sempre està buscant noves aventures</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/cabra.mp3')">Audio</ion-button>
      </ion-item>

      <ion-item>
        <ion-thumbnail slot="start">
          <img src="/animals/conill.jpg" />
        </ion-thumbnail>
        <ion-label>
          <h2>CONILL</h2>
          <p>Àgil i nerviós, el conill salta de manera graciosa pel camp</p>
        </ion-label>
        <ion-button slot="end" size="default" @click="playAudio('/audio/conill.mp3')">Audio</ion-button>
      </ion-item>
    </ion-list>
  </ion-content>
</template>

<script lang="ts">
import {
  IonContent,
  IonHeader,
  IonItem,
  IonLabel,
  IonList,
  IonThumbnail,
  IonTitle,
  IonToolbar,
  IonButton
} from '@ionic/vue'
import { defineComponent } from 'vue'

export default defineComponent({
  components: {
    IonContent,
    IonHeader,
    IonToolbar,
    IonTitle,
    IonList,
    IonItem,
    IonLabel,
    IonThumbnail,
    IonButton
  },
  methods: {
    playAudio(path: string) {
      const audio = new Audio(path)
      audio.play()
    }
  }
})
</script>

<style scoped>
ion-content {
  overflow-y: auto;
  padding-bottom: 20px; 
}
</style>
