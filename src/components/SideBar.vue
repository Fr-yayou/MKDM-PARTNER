<template>
  <div class="sideBar">
      <div>
          <h3>Logo</h3>
      </div>
      <div class="container-Link">
          <ul class="link-dashboard">
              <div>
                    <v-icon>{{icons.mdiViewDashboardOutline}}</v-icon>
                    <li>Dashboard</li>
              </div>
              <div>
                  <v-icon>{{icons.mdiCreditCardOutline}}</v-icon>
                  <li>Billing</li> 
              </div>
              <div>
                  <v-icon>{{icons.mdiFormatListBulleted}}</v-icon>
                  <li>Task</li> 
              </div>
          </ul>
          <ul class="link-profile">
              <div>
                  <v-icon>{{icons.mdiTuneVerticalVariant}}</v-icon>
                  <li>Setting</li> 
              </div>
              <div>
                  <v-icon>{{icons.mdiLogout}}</v-icon>
                  <li>Log out</li> 
              </div>
          </ul>
      </div>
  </div>
</template>

<script>
import  {   mdiViewDashboardOutline,mdiCreditCardOutline, 
            mdiTuneVerticalVariant, 
            mdiStickerPlusOutline,
            mdiFormatListBulleted,
            mdiLogout,
        } from '@mdi/js'

export default {
    name:"SideBar",

    data(){
        return{
            icons:{
                mdiViewDashboardOutline,
                mdiCreditCardOutline, 
                mdiTuneVerticalVariant, 
                mdiStickerPlusOutline,
                mdiLogout,
                mdiFormatListBulleted

            }
        }
    }
}
</script>

<style scoped>
.sideBar{
    padding-left: 35px;
    padding-top: 60px;
    padding-bottom:60px
}

.container-Link{
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;

}

.link-dashboard{
    list-style: none;
    padding-left: 0px;
    height: 170px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-top: 30px;

}
.link-dashboard div:first-child{
    border-right: 3px solid #FFAB91;
    height: 35px;
    align-items: flex-end;
}

.link-dashboard div:first-child span{
    background-color:#FFAB91;
    border-radius:5px;
    color:#FFCCBC;
    opacity: 0.8 ;
}
.link-profile{
    list-style: none;
    padding-left: 0px;
    
}
.link-profile div:first-child{
    padding-bottom: 25px;
}

.link-dashboard div{
    display: flex;
    
}
.link-dashboard div li{
    padding-left: 10px;   
}
.link-profile div li{
    padding-left: 10px;   
}
.link-profile div{
    display: flex;

}



</style>