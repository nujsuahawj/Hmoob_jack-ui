<template>
    <v-footer padless>
        <v-col lg="12">
            <v-row justify="center">
                <v-col lg="4" class="text-center">
                    <v-toolbar-title>Jack Sainther</v-toolbar-title>
                    <v-card-text>
                        <v-btn
                                v-for="icon in icons"
                                :key="icon"
                                class="mx-4 black--text"
                                icon
                        >
                            <v-icon size="24px">
                                {{ icon }}
                            </v-icon>
                        </v-btn>
                    </v-card-text>
                    <v-subheader>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi autem blanditiis
                        deserunt eius impedit nihil obcaecati perspiciatis quo sunt voluptate.
                    </v-subheader>
                    <v-form class="mt-4">
                        <v-text-field label="Email" outlined dense />
                        <v-btn rounded color="success">Subscribe us</v-btn>
                    </v-form>
                </v-col>

            </v-row>
            <div class="mt-10">
                <v-divider></v-divider>
                <v-subheader>
                    © Copyright Web Burden. All Rights Reserved {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
                    <v-spacer />
                    <strong>Designed by Tushar Ahmed</strong>
                </v-subheader>
            </div>
        </v-col>
    </v-footer>
</template>

<script>
    export default {
        name: "Footer",
        data() {
            return {
                icons: [
                    'mdi-facebook',
                    'mdi-twitter',
                    'mdi-linkedin',
                    'mdi-instagram',
                ],
            }
        }
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