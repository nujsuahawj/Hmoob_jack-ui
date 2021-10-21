<template>
    <v-container class="pt-15">
        <v-row>
            <v-col lg="6">
                <h2 class="intro-text">ຍິນດີຕ້ອນຮັບສູ່ jack ui</h2>
                <p class="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias autem beatae ex exercitationem fuga
                    fugiat nobis officiis quia rerum sit?</p>
                <v-btn color="success" class="white--text mr-10" rounded>ເລີມເລີຍ</v-btn>
                <v-btn color="indigo" class="white--text" rounded>
                    <v-icon>mdi-play-circle</v-icon> ເບິ່ງຕົວຢ່າງ
                </v-btn>
            </v-col>
            <v-col lg="6">
                <img width="100%" src="./../assets/hero-img.png" alt="">
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "HeroComponent"
    }
</script>

<style scoped>
    h2.intro-text {
        font-size: 60px;
        font-weight: bold;
        color: #444;
    }
    p.description {
        font-size: 19px;
        margin: 32px 0px;
        color: #444444ba;
        font-family: 'Noto Sans Lao', sans-serif;
    }
    .v-toolbar__title {
        font-size: 32px;
        color: #4caf50;
        font-weight: 700;
        font-family: 'Noto Sans Lao', sans-serif;
    }
  .v-list-item{
    font-family: 'Noto Sans Lao', sans-serif;
  }
  .v-btn{
    font-family: 'Noto Sans Lao', sans-serif;
  }
  .intro-text{
      font-family: 'Noto Sans Lao', sans-serif;
  }
</style>