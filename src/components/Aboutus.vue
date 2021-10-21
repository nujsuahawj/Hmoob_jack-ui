<template>
    <v-container>
        <v-row>
            <v-col lg="6">
                <img src="./../assets/about-us.jpg" alt="">
            </v-col>
            <v-col lg="6">
                <v-subheader class="text-h4">ກ່ຽວກັບ</v-subheader>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Assumenda delectus distinctio eligendi esse
                    explicabo hic perferendis provident repudiandae suscipit ullam.</p>
                <v-list>
                    <v-list-item>
                        <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                        <v-list-item-subtitle>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, ut.
                        </v-list-item-subtitle>
                    </v-list-item>
                    <v-list-item>
                        <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                        <v-list-item-subtitle>Lorem ipsum dolor sit amet, consectetur adipisicing</v-list-item-subtitle>
                    </v-list-item>
                    <v-list-item>
                        <v-icon color="success" class="mr-3"> mdi-check-all</v-icon>
                        <v-list-item-subtitle>Lorem ipsum dolor sit amet,</v-list-item-subtitle>
                    </v-list-item>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam architecto commodi consequatur
                        consequuntur doloribus ducimus ea eius est et iusto laboriosam nesciunt non, numquam odio
                        pariatur praesentium quas qui quidem quod saepe sequi sit tenetur voluptates. Minus non quia
                        recusandae!</p>
                </v-list>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "Aboutus"
    }
</script>

<style scoped>
    p.v-col{
        font-family: 'Noto Sans Lao', sans-serif;
    }
    .text {
        font-family: 'Noto Sans Lao', sans-serif;
    }
  .v-list-item{
    font-family: 'Noto Sans Lao', sans-serif;
  }
  .intro-text{
      font-family: 'Noto Sans Lao', sans-serif;
  }
</style>