<template>
<div class="portfolioWrap">
<v-container>
  <v-layout row wrap>
    <v-flex xl 12 sm6 md4 lg4 v-for="(obj, key2) in portfolios" :key="key2">
     <v-card
    max-width="344"
    class="mx-auto"
  >
    <v-list-item>
      <v-list-item-avatar color="grey"></v-list-item-avatar>
      <v-list-item-content>
        <v-list-item-title class="headline">{{ obj.caption }}</v-list-item-title>
        <v-list-item-subtitle>by Kurt Wagner</v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>

    <v-img class="imgPortoflio" :src='obj.img'
      height="194"
    ></v-img>

    <v-card-text>
      Visit ten places on our planet that are undergoing the biggest changes today.
    </v-card-text>

    <v-card-actions>
      <v-btn
        text
        color="deep-purple accent-4"
      >
        Read
      </v-btn>
      <v-btn
        text
        color="deep-purple accent-4"
      >
        Bookmark
      </v-btn>
      <div class="flex-grow-1"></div>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-share-variant</v-icon>
      </v-btn>
    </v-card-actions>
  </v-card>
  </v-flex>
  </v-layout>
</v-container>
</div>

             
</template>

<script>


export default {
   
  data: ()=> ({
    show: false,
    portfolios: [
      {
        img:require('../assets/img/definov-group.png'),
        caption: 'Wordpress',
        title: 'Definov-group'
      },
      {
        img:require('../assets/img/definov-formation.png'),
        caption: 'Moodle',
        title: 'Definov-formation'
      },
      {
        img:require('../assets/img/Lyon.png'),
        caption: 'JavaScript + API JCDecaux',
        title: 'Carte intéractive de location de vélo + gestion des réservations'
      },
      {
        img:require('../assets/img/projet4.png'),
        caption: 'PHP & MySQL',
        title: 'Création d’un blog pour un écrivain'
      },
      {
        img:require('../assets/img/Aquattitude.png'),
        caption: 'Wordpress',
        title: 'Conception et réalisation du site Aquattitude.fr'
      },
      {
        img:require('../assets/img/Securizme.png'),
        caption: 'Wordpress',
        title: 'Conception et réalisation du site Securizme.fr'
      },
        {
        img:require('../assets/img/webAgency.png'),
        caption: 'HTM5 & CSS3',
        title: 'Réalisation du site internet d\'une Web agency'
      }


    ]
  })
    
}
</script>

<style>
v-btn__content{color: black !important;} 


</style>