<template>
    <v-container class="my-15">
        <v-row justify="center">
            <v-col lg="12" class="text-center">
                <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsam, quam!</p>
            </v-col>
            <v-col lg="12">
                <div class="text-center">
                    <v-chip @click="activePortfolio = 'webapp'" :color="activePortfolio === 'webapp'? 'success':''" class="mx-5">Web App</v-chip>
                    <v-chip @click="activePortfolio = 'mobileapp'" :color="activePortfolio === 'mobileapp'? 'success':''" class="mx-5">Mobile App</v-chip>
                    <v-chip @click="activePortfolio = 'desktopapp'" :color="activePortfolio === 'desktopapp'? 'success':''" class="mx-5">Desktop App</v-chip>
                </div>
            </v-col>
            <slot v-if="activePortfolio === 'webapp'">
                <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex">
                    <v-card>
                        <v-img
                                :src="web.image"
                                class="white--text align-end"
                                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                                height="200px"
                        >
                            <v-card-title>{{web.title}}</v-card-title>
                        </v-img>
                    </v-card>
                </v-col>
            </slot>
            <slot v-if="activePortfolio === 'mobileapp'">
                <v-col lg="3" v-for="(mobile,mobileindex) in mobileApps" :key="mobileindex">
                    <v-card>
                        <v-img
                                :src="mobile.image"
                                class="white--text align-end"
                                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                                height="200px"
                        >
                            <v-card-title>{{mobile.title}}</v-card-title>
                        </v-img>
                    </v-card>
                </v-col>
            </slot>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "Portfolio",
        data(){
            return{
                activePortfolio:'webapp',
                webApps:[
                    {title:'Web App 1',image:'https://res.cloudinary.com/practicaldev/image/fetch/s--gJHvKBc---/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1srpidiu14okwwtvwkhn.png'},
                    {title:'Web App 2',image:'https://p.kindpng.com/picc/s/127-1272110_web-application-transparent-hd-png-download.png'},
                    {title:'Web App 3',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Web App 4',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRvmof4X00_zX5j8B2Km_Taa6nZy-0YdEx8E0TKE38oObAX7qlOLZDVaXBJdmqrqfNBL2o&usqp=CAU'},
                    {title:'Web App 5',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Web App 6',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRW9Q_S3C6j2aSyMesVRlrNrPClSyPmeJNnv8624RPn43-YC_4vu9wyuz8dOKQFFSD8q28&usqp=CAU'},
                    {title:'Web App 7',image:'https://p.kindpng.com/picc/s/127-1272110_web-application-transparent-hd-png-download.png'},
                ],
                mobileApps:[
                    {title:'Mobile App 1',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 2',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 3',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 4',image:'https://cdn.dribbble.com/users/404195/screenshots/13892505/media/541a6221e947a980b8f001b3837a0ab1.png?compress=1&resize=400x300'},
                    {title:'Mobile App 5',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Mobile App 6',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRW9Q_S3C6j2aSyMesVRlrNrPClSyPmeJNnv8624RPn43-YC_4vu9wyuz8dOKQFFSD8q28&usqp=CAU'},
                    {title:'Mobile App 7',image:'https://cdn.dribbble.com/users/404195/screenshots/13892505/media/541a6221e947a980b8f001b3837a0ab1.png?compress=1&resize=400x300'},
                ]
            }
        }
    }
</script>

<style scoped>

</style>