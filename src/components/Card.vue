<template>
  <div class="card">
      <div class="card-header">
          <h4>Your team</h4>
          <v-checkbox
            value="1"
            label="Completed tasks"
            type="checkbox"
            required
          ></v-checkbox>
      </div>
      <div>
          <div class="table-head">
                    <p>Ressource</p>
                    <p>Current</p>
                    <p>Actions</p>
          </div>
          <div class="table-body">
              <div class="profile-info">
                  <div>
                      <img class="picture" src="../assets/male.svg" alt="picture">
                      <div class="infos">
                          <h4>Project Manager</h4>
                          <span>john Smith</span>
                          <span>35 Hours</span>
                      </div>
                  </div>
              </div>
              <div>
                  <h5>Phase 1 of the CMS</h5>
                  <div class="progressBar">
                    <div class="progress"><span class="pointer">50%</span></div>
                  </div>
              </div>
              <div class="actions">
                  <v-icon>{{icons.mdiClockTimeEightOutline }}</v-icon>
                  <v-icon>{{icons.mdiTrashCanOutline}}</v-icon>
              </div>
          </div>
          <div id="elevate" class="table-body">
              <div class="profile-info">
                  <div>
                      <img class="picture" src="../assets/femme.svg" alt="picture">
                      <div class="infos">
                          <h4>Senior Developer</h4>
                          <span>Mike Brown</span>
                          <span>50H</span>
                      </div>
                  </div>
              </div>
              <div>
                    <h5>Setting up Dev/Prod/Test Environements</h5>
                    <div class="progressBar">
                        <div class="progressTwo"><span class="pointer">63%</span></div>
              </div>
              </div>
              <div class="actions">
                  <v-icon>{{icons.mdiClockTimeEightOutline }}</v-icon>
                  <v-icon>{{icons.mdiTrashCanOutline}}</v-icon>
              </div>
          </diV>
          <div class="table-body">
              <div class="profile-info">
                  <div>
                      <img class="picture" src="../assets/femme.svg" alt="picture">
                      <div class="infos">
                          <h4>Web Designer</h4>
                          <span>Jane Doe</span>
                          <span>25H</span>
                      </div>
                  </div>
              </div>
              <div>
                  <h5>Logo Design</h5>
                  <div class="progressBar">
                  <div class="progressThree"><span id="none" class="pointer">100%</span></div>
                  <div class="check">
                      <v-btn color="#A5D6A7"   small elevation="2" class="white--text"><v-icon color="white">{{icons.mdiCheckBold}}</v-icon>Approve</v-btn>
                      <span>Dispute</span>
                  </div>
              </div>
              </div>
              <div class="actions">
                  <v-icon>{{icons.mdiClockTimeEightOutline }}</v-icon>
                  <v-icon>{{icons.mdiTrashCanOutline}}</v-icon>
              </div>
          </diV>
      </div>
  </div>
</template>

<script>
import { mdiTrashCanOutline } from '@mdi/js';
import { mdiClockTimeEightOutline } from '@mdi/js';
import { mdiCheckBold } from '@mdi/js';
export default {
    name:"Card",
    data(){
        return{
            icons:{mdiTrashCanOutline, mdiClockTimeEightOutline,mdiCheckBold }
        }
    }


}
</script>

<style scoped>
.card-header{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.card{
    margin-left: 30px;
    margin-right: 30px;
    height:350px
}
.table-head {
    display: flex;
    height: 40px;
    background-color: #eaf1f8;
    border-radius: 10px;
    justify-content: space-between;
    align-items: center;
}
.table-head p {
    margin-bottom: 0px;
}

.table-body{
    display: flex;
    justify-content: space-between;
    margin-top:10px;
    padding-right: 15px;
    padding-left: 15px;
    margin-top: 10px;
}
.picture{
    width: 45px;
    margin-right: 15px;
}

.profile-info{
    width: 33%;
}

.profile-info div:first-child{
    display: flex;
}
.infos{
    display: flex;
    flex-direction: column;
}
.table-head :first-child{
    padding-left: 15px;
}
.table-head :last-child{
    padding-right: 15px;
}
#elevate{
   box-shadow:rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;;
   border-radius: 20px;
}

.progressBar{
    height: 20px;
    width: 230px;
    margin-right: 60px;
    background-color:#eaf1f8;
    align-self: center;
    border-radius:20px
}

.progress{
    height: 20px;
    width: 120px;
    background-color: #FFAB91;
    border-radius:20px  
}

.progressTwo{
    
    height: 20px;
    width: 120px;
    background-color: #FFAB91;
    border-radius:20px  

}
.progressThree{
    height: 20px;
    width: 100%;
    background-color: #B39DDB;
    border-radius:20px  
}

.pointer{
    background-color: white;
    position: absolute;
    margin-left: 113px;
    height: 20px;
    font-size:15px;

}

.actions{
    display: flex;
    align-items: center;
    width: 10%;
    justify-content: space-around;
}

.actions span:first-child{
    background-color:#CFD8DC;
    padding:1px;
    border-radius:5px
}

.actions span:last-child{
    background-color:#FFCDD2;
    color:#EF5350;
    padding:1px;
    border-radius:5px
}

.infos span{
    font-size:12px
}
#none{
    display: none;
}

.check{
    margin-top: 5px;
}
.check button{
    margin-right: 5px;
}
.check span{
    font-size: 15px;
}







</style>