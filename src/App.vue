<template>
  <v-app>
    <v-main>
      <div class="container-mainView">
        <SideBar class="sideBar"/>
        <div class="dashboard-container">
          <Dashboard/> 
        </div>
        <SideBarTwo/>
      </div>
    </v-main>
  </v-app>
</template>

<script>

import SideBar from "./components/SideBar"
import Dashboard from "./components/DashBoard"
import SideBarTwo from "./components/SideBarTwo"

export default {
  name: 'App',

  components: {
    SideBar,
    Dashboard,
    SideBarTwo
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped>
#app{
  background-color: #E0E0E0;
}
.container-mainView{
  display: flex;
  background-color: white;
}
.sideBar{
  width: 20%;
}

.dashboard-container{
    width: 60%;
    height: 100vh;
    padding-top: 20px;
    padding-bottom: 20px;
}
</style>
