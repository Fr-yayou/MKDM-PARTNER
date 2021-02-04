<template>
  <div class="sideTwo">
      <div class="container-title">
          <div>
              <p>Current balance <span>$100</span></p>
              <p>Increase Balance For FREE</p>
          </div>
          <v-btn elevation="2" color="white"  fab medium tile><v-icon>{{icons.mdiBellRingOutline}}</v-icon></v-btn>
          <v-btn elevation="2" color="#FFAB91" medium fab tile ><v-icon color="white">{{icons.mdiAccount}}</v-icon></v-btn>
      </div>
      <div class="container-search">
          <h4>Ressources chat</h4>
          <div class="container-seearch">
              <div class="search"></div>
              <div class="result">
                  <div>
                      <img class="picture" src="../assets/male.svg" alt="picture">
                       <h5>John Smith</h5>
                  </div>
                  <div>
                      <img class="picture" src="../assets/femme.svg" alt="picture">
                      <h5>Jane Due</h5>
                  </div>
                  <div>
                      <img class="picture" src="../assets/male.svg" alt="picture">
                      <h5>Mike Brown</h5>
                  </div>
              </div>
          </div>
      </div>
      <div class="line-breaker"></div>

  </div>
</template>

<script>
import { mdiBellRingOutline,mdiAccount  } from '@mdi/js';
export default {
    name:"SideBarTwo",

    data(){
        return{
            icons:{mdiBellRingOutline,mdiAccount}
        }
    }
}
</script>

<style scoped>
.sideTwo{
    width: 30%;
}
.container-title{
    padding-top:60px;
    display: flex;
    justify-content: flex-end;
    padding-right: 25px;
    padding-left: 50px;
    justify-content: space-around;

}
.container-title button{
    border-radius: 15px
}
.container-title div p{
    margin-bottom: 0px;
    font-size: 13px;
}
.container-title div p span{
    font-weight: bold;
    font-size:18px
    
}
.container-title div p:last-child{
    color:#FFAB91;  
}

.container-title div {
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
}

.container-search{
    padding-left: 35px;
    padding-top: 40px;
    padding-right: 25px;
}
.container-search h4{
    padding-bottom: 20px;
}

.search{
    height: 35px;
    border-radius: 20px;
    border:1px solid lightgray ;
    background-color:  #eaf1f8;
    margin-bottom: 20px;
}

.result{
    padding-bottom: 50px;
}

.result div{
    display: flex;
    background-color: white;
    border-radius: 20px;
    height: 55px;
    margin-bottom: 20px;
    box-shadow:rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;;
    border-radius: 20px;   
}
.result div h5{
    align-self: center;
}

.picture{
    width: 35px;
    margin-right: 15px;
    margin-left: 20px;
}

.line-breaker{
    height: 1px;
    background-color: lightgrey;
    margin-left: 35px;
    margin-right: 35px;
}



</style>