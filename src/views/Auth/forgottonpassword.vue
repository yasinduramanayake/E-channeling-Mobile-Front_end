<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar color="tertiary">
        <ion-buttons slot="start">
          <ion-back-button text="" default-href="/"></ion-back-button>
        </ion-buttons>
        <ion-title style="padding-left:70px">E-channeling</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <ion-row>
        <Logo />
      </ion-row>

      <br />

      <ion-item>
        <ion-label position="stacked">E-mail</ion-label>
        <ion-input placeholder="E-mail"></ion-input>
      </ion-item>
      <br />
      <br />
      <br />

      <br />

      <div style="margin-left:5%;, margin-right:5%;">
        <ion-button
          color="tertiary"
          @click="() => router.push('/login')"
          expand="block"
          >Send Link
        </ion-button>
      </div>
    </ion-content>
  </ion-page>
</template>
<script>
import {
  IonPage,
  IonContent,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonButtons,
  IonBackButton,
  IonInput,
  IonLabel,
  IonItem,
  IonButton,
  IonRow,
} from "@ionic/vue";
import login from "@/router/modules/login";
import { useRouter } from "vue-router";
import Logo from "@/views/components/logo.vue";
export default {
  name: login,
  components: {
    IonPage,
    IonContent,
    IonHeader,
    IonTitle,
    IonToolbar,
    IonButton,
    IonButtons,
    IonBackButton,
    IonInput,
    IonLabel,
    IonItem,

    Logo,
    IonRow,
  },

  setup() {
    const router = useRouter();
    return {
      router,
    };
  },
};
</script>

<style scoped>
.txt_forgot_password {
  margin-top: 2%;
  padding-left: 30%;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: medium;
}

.signup {
  padding-left: 14%;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: medium;
  font-weight: bold;
}
</style>
