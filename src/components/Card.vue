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
              <p>Hello</p>
              <p>Hello</p>
              <p>Hello</p>
          </diV>
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
              <p>Hello</p>
              <p>Hello</p>
              <p>Hello</p>
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
              <p>Hello</p>
              <p>Hello</p>
              <p>Hello</p>
          </diV>
      </div>
  </div>
</template>

<script>
export default {
    name:"Card",


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




</style>