<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    
    <ion-content :fullscreen="true">
      <ion-header collapse="condense" class="ion-no-border">
        <ion-toolbar>
          <ion-title size="large">Home</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-grid>
        <ion-row>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Kolam</ion-card-subtitle>
                <ion-card-title><b>10</b></ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Kolam Aktif</ion-card-subtitle>
                <ion-card-title>8</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Ikan Hidup</ion-card-subtitle>
                <ion-card-title>182 <span>Ekor</span></ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Ikan Mati</ion-card-subtitle>
                <ion-card-title ><b>89 Ekor</b></ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Panen 2022</ion-card-subtitle>
                <ion-card-title><b>109 Kg</b></ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="RowInfo">
              <ion-card-header>
                <ion-card-subtitle>Total Pakan</ion-card-subtitle>
                <ion-card-title>223 Kg</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>

      <div class="text">
        <h3>TOTAL BERAT IKAN</h3>
      </div>
      <ion-row>
          <ion-col>
            <ion-card class="RowBerat">
              <img alt="Lele" src="https://img.freepik.com/premium-vector/catfish-vector-illustration_175152-258.jpg?strip=all" style="width: 500px;height: 150px;"/>
              <ion-card-header>
                <ion-card-title>Ikan Lele</ion-card-title>
                <ion-card-subtitle><span class="blue">200 Kg</span></ion-card-subtitle>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="RowBerat">
              <img alt="Nila" src="https://1.bp.blogspot.com/-dHe3dP4w4qA/WwhdaIk3VvI/AAAAAAAABeU/QPy2RklSfRgOQ1R2Dg6Fb-sv6B_OKVGOgCLcBGAs/s1600/11.jpg" style="width: 500px;height: 150px;"/>
              <ion-card-header>
                <ion-card-title>Ikan Nila</ion-card-title>
                <ion-card-subtitle><span class="blue">220 Kg</span></ion-card-subtitle>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
        
      <div class="text">
        <h3>KUALITAS AIR</h3>
      </div>
      <ion-row>
          <ion-col>
            <ion-card class="RowKualitas">
              <ion-card-header>
                <ion-card-title><b>pH</b></ion-card-title>
                <ion-card-subtitle>Normal: <span class="blue">5 Kolam</span></ion-card-subtitle>
                <ion-card-subtitle>Abnormal: <span class="blue">5 Kolam</span></ion-card-subtitle>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col>
            <ion-card class="RowKualitas">
              <ion-card-header>
                <ion-card-title><b>DO</b></ion-card-title>
                <ion-card-subtitle>Normal: <span class="blue">5 Kolam</span></ion-card-subtitle>
                <ion-card-subtitle>Abnormal: <span class="blue">5 Kolam</span></ion-card-subtitle>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar,IonGrid,IonCol,IonRow,IonCard } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomePage',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    IonGrid,
    IonCol,
    IonRow,
    IonCard
  }
});
</script>

<style scoped>
 ion-title{
  font-weight: bold;
  font-size: 25px;
 }

 ion-card{
  border-radius: 15px;
 }

 ion-card-title{
  color: black;
  font-weight: bold;
  font-size: 25px;
 }

 ion-card-subtitle{
  color: black !important;
  font-weight: bold;
  font-size: 20px;
 }

 .blue{
  color: lightskyblue;
  font-weight: bold;
 }

 .text{
  color: white;
  padding-left: 17px;
  font-weight: bold;
 }

 .RowInfo {
  background-color: white;
  color: black;
  font-weight: bold;
  font-size: 30px;
 }

 .RowBerat{
  background-color: white;
 }

 .RowKualitas{
  background-color: white;
 }
</style>
