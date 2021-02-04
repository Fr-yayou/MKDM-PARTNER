<template>
  <div class="dashboard">
      <div class="container-dashboard">
        <h1>Team Service</h1>
        <div class="container-btn">
            <v-btn  elevation="5"  color="white"><v-icon>{{icons.mdiAccountMultiplePlusOutline }}</v-icon><span class="btnText">New ressource</span></v-btn>
            <v-btn  elevation="5"  color="white"><v-icon>{{icons.mdiStickerPlusOutline}}</v-icon><span class="btnText">New Task</span></v-btn>
            <v-btn  elevation="5" color="white"><v-icon>{{icons.mdiFormatListBulleted}}</v-icon><span class="btnText">All tasks</span></v-btn>
            <v-btn  elevation="5"  color="white"><v-icon>{{icons.mdiCreditCardOutline}}</v-icon><span class="btnText">Billing</span></v-btn>
        </div>
        <div class="container-card">
            <Card/>
        </div>
        <!-- <SecondCard/> -->
      </div>
  </div>
</template>

<script>
import Card from "../components/Card"
// import SecondCard from "../components/SecondCard"
import {
    mdiAccountMultiplePlusOutline,mdiFormatListBulleted,
    mdiCreditCardOutline,mdiStickerPlusOutline   
} from '@mdi/js'
export default {
    name:"Dashboard",

    components:{
        Card,
        // SecondCard
    },

    data(){
        return{
            icons:{mdiAccountMultiplePlusOutline,mdiFormatListBulleted,
                mdiCreditCardOutline,
                mdiStickerPlusOutline   
             }
        }
    }
}
</script>

<style scoped>
.dashboard{
    background-color:#eaf1f8; ;
    height: 100%;
    border: 1px solid #eaf1f8;;
    border-radius:30px

}
.btnText{
    font-size:10px
}

.container-btn{
    display: flex;
    justify-content: space-between;
    width: 75%;
    padding-top: 35px;
}

.container-dashboard{
    margin-left: 30px;
    margin-right:30px
}
.container-dashboard h1{
    padding-top: 40px;
}

.container-card{
    margin-top: 50px;
    background-color: white; 
    border-radius:15px
}
</style>



