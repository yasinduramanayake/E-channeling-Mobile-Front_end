<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar color="tertiary">
        <ion-buttons slot="start">
          <ion-back-button text="" default-href="/"></ion-back-button>
        </ion-buttons>
        <ion-title style="padding-left:70px">Ayurvedic Hospitals</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <ion-grid>
        <ion-row>
          <ion-col> </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <img class="logo" src="assets/echannelling.png" />
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col>
            <ion-card>
              <ion-card-header>
                <ion-card-title>Ayurvedic Hospital</ion-card-title>
                <ion-card-subtitle>Doctor Channeling</ion-card-subtitle>
               <br>
              </ion-card-header>

              <ion-card-content>
                <ion-text color="dark">
                  <h2>Doctor's Name</h2>
                </ion-text>
                <ion-input
                  placeholder="Enter Doctor's Name"
                  background="Blue"
                ></ion-input>
                <br />
                <br />

                <ion-list>
                  <ion-text color="dark">
                    <h2>Specialization</h2>
                  </ion-text>

                  <ion-item>
                    <ion-select
                      value="brown"
                      placeholder="Select The Specialization"
                      ok-text="OK"
                      cancel-text="Cancel"
                    >
                      <ion-select-option value="blonde"
                        >Aesthetic Cosmetologist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Aesthetic Medicine and Cosmetologist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Anaesthetist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Audiologist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Basteriologist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Cardiologist</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >Chest Physican</ion-select-option
                      >
                      <ion-select-option value="blonde"
                        >General Physican</ion-select-option
                      >
                    </ion-select>
                  </ion-item>
                </ion-list>
                <br />
                <br />
                <br />
                <br />

                <ion-button
                  expand="block"
                  color="tertiary"
                  @click="() => router.push('/list2')"
                  >Search</ion-button
                >
                <br />
                <br />
              </ion-card-content>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<script>
import { useRouter } from "vue-router";
import {
  IonPage,
  IonContent,
  IonCard,
  IonInput,
  IonGrid,
  IonButtons,
  IonRow,
  IonCol,
  IonToolbar,
  IonButton,
  IonBackButton,
  IonHeader,
  IonTitle,
  IonCardHeader,
  IonCardTitle,
  IonCardSubtitle,
  IonCardContent,
  IonText,
  IonList,
  IonItem,
  IonSelect,
  IonSelectOption,
} from "@ionic/vue";

export default {
  components: {
    IonPage,
    IonContent,
    IonCard,
    IonGrid,
    IonButtons,
    IonInput,
    IonRow,
    IonCol,
    IonToolbar,

    IonButton,
    IonBackButton,
    IonHeader,
    IonTitle,
    IonCardHeader,
    IonCardTitle,
    IonCardSubtitle,
    IonCardContent,
    IonText,
    IonList,
    IonItem,
    IonSelect,
    IonSelectOption,
  },
  methods: {},

  setup() {
    const router = useRouter();
    return {
      router,
    };
  },
};
</script>

<style>
.logo {
  padding-top: 2%;
  margin-left: 32%;
  height: 120px;
  width: 120px;
}

ion-input {
  border-radius: 10px;
  padding-right: 30px;
  padding-left: 30px;
  font-size: 0.9em;
  border: 1px solid #f1f1f1;
  --background: rgb(219, 219, 219);
  /* height: 10%; */
  max-width: 100vw;
  max-height: 10vh;
}
</style>
