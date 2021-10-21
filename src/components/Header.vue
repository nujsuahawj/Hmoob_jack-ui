<template>
  <v-app-bar
            style="padding: 0px 90px"
            app
            color="white"
            light
            elevation="6"
            elevate-on-scroll
    >
        <v-toolbar-title>Jack Sainther</v-toolbar-title>
        <v-spacer />
        <v-list class="d-flex align-center">
            <v-list-item link v-for="(menu,index) in menus" :key="index" :to="menu.route">
                <v-list-item-title>{{menu.title}}</v-list-item-title>
            </v-list-item>
            <v-btn text class="mx-10" >
                <v-icon>mdi-magnify</v-icon>
            </v-btn>
            <v-btn outlined color="success">ເຂົ້າສູ່ລະບົບ</v-btn>
        </v-list>

  </v-app-bar>
</template>

<script>
    export default {
        name: "Header",
        data(){
            return{
                menus:[
                    {title:'ໜ້າລັກ',      route:'home'},
                    {title:'ກ່ຽວກັບ',  route:'about-us'},
                    {title:'ໂປຣໄຟຂອງພວກເຮົາ', route:'protfolio'},
                    {title:'ໂປຣແຈັກ',   route:'project'},
                    {title:'ຮູບພາບ',   route:'galley'},
                    {title:'ຕິດຕໍ',   route:'contact'},
                ]
            }
        }
    }
</script>
<style>
    .v-toolbar__title {
        font-size: 32px;
        color: #4caf50;
        font-weight: 700;
        font-family: cursive;
    }
  .v-list-item{
    font-family: 'Noto Sans Lao', sans-serif;
  }
  .v-btn{
    font-family: 'Noto Sans Lao', sans-serif;
  }
</style>
