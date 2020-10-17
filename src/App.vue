<template>
  <ion-app>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tasks</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content fullscreen="true">
<!-- router -->
    <ion-router-outlet />

      <ion-toolbar>
        <ion-segment value="all">
          <ion-segment-button value="pending">Pending</ion-segment-button>
          <ion-segment-button value="completed">Completed</ion-segment-button>
          <ion-segment-button value="favorites">Favorites</ion-segment-button>
        </ion-segment>
      </ion-toolbar>

      
    </ion-content>

    <ion-footer>
      <ion-toolbar>
        <ion-title>
          Click to Add Text
        </ion-title>
        <ion-buttons slot="end">
          <ion-button id="changeText" onClick="toggleText()">
            <ion-icon slot="start" name="refresh"></ion-icon>
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-footer>
  </ion-app>
</template>

<script lang="ts">
import { IonApp, IonRouterOutlet,IonToolbar,IonHeader,IonTitle,IonIcon,IonSegment,IonSegmentButton,IonContent,IonButton,IonButtons,IonFooter } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet,IonToolbar,
IonHeader,
IonTitle,
IonIcon,IonSegment,IonSegmentButton,IonContent,IonButton,IonButtons,IonFooter
  }
});
</script>