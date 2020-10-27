<template>
  <ion-page>
    <ion-header :translucent="false" >
      <ion-toolbar>
        <ion-title> DepLog</ion-title>
      </ion-toolbar>
    </ion-header>
    
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>
    
      <div id="container">
        <ion-card style='width: 400px; height:200px; background-color:lightblue'>
          <ion-card-header>
            <ion-card-subtitle><!-- subtitulo va arriba del titulo --></ion-card-subtitle>
            <ion-card-title>Ingrese datos para iniciar sesión</ion-card-title>
          </ion-card-header>

          <ion-card-content>
            
            <ion-card style='width: 250px; height:40px'>
              <!-- espacio para ingresar dato -->
              <ion-input placeholder="Correo" ></ion-input>
            </ion-card>
            <ion-card style='width: 250px; height:40px'>
              <ion-input placeholder="Contraseña"></ion-input>
            </ion-card>

          </ion-card-content>
        </ion-card>
        <p>Start with Ionic <a target="_blank" rel="noopener noreferrer" href="https://ionicframework.com/docs/components">UI Components</a></p>
        
        
        
      </div>
    </ion-content>
    <div class="navbar">
      <a href="#home" class="active">Home</a>
      <a href="#Contacto">Contacto</a>
      <a target="_blank" rel="noopener noreferrer" href="https://www.youtube.com/watch?v=WF8l9cPmmJI&ab_channel=MiguelRam%C3%ADrez">Sobre nosotros</a>
    </div>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar,IonLabel , IonInput, IonItem,  IonCard, IonCardContent, IonCardSubtitle, IonCardTitle, IonIcon } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    
    IonInput,
    
    IonCard,
    IonCardContent,
    IonCardSubtitle,
    IonCardTitle,
  }
});
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 35%;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}

/* Place the navbar at the bottom of the page, and make it stick */
.navbar {
  background-color: rgb(253, 252, 252);
  overflow: hidden;
  position: fixed;
  bottom: 0;
  width: 100%;
}

/* Style the links inside the navigation bar */
.navbar a {
  float: left;
  display: block;
  color: #030000;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.navbar a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.navbar a.active {
  background-color: #ffffff;
  color: rgb(0, 0, 0);
}
</style>