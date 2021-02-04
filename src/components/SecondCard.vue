<template>
  <div class="container-SecondCard">
      <h3>Yours Tasks</h3>

      <div>
           <div class="headTable">
               <p>Task Name</p>
               <p>Progress</p>
               <p>Assigned To</p>
           </div>
           <div class="bodyTable">
               <h4>Setup Source Control Branching</h4>
               <p>Hello</p>
               <p>Hello</p>
           </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"SecondCard"
}
</script>

<style scoped>
.headTable{
    display: flex;
    height: 40px;
    background-color: #eaf1f8;
    border-radius: 10px;
    justify-content: space-between;
    align-items: center;
}

.headTable p{
    margin-bottom:0px
}
.headTable p:first-child{
    padding-left:15px
}
.headTable p:last-child{
    padding-right:15px
}
.bodyTable{
    display:flex;
    justify-content: space-between;
}

.container-SecondCard{
    padding-left: 30px;
    padding-right: 30px;
}




</style>