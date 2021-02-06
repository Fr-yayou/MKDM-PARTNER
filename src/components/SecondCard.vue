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
                   <div class="progressBar">
                    <div class="progressTwo"><span class="pointer">0%</span></div>
                    </div>
               <div class="me">
                   <img class="picture" src="../assets/male.svg" alt="picture">
                   <span>Mike Brown</span>
               </div>
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
    align-items: center;
    padding-bottom: 10px;
    padding-top: 10px;
}

.bodyTable h4{
    width: 40%;
    margin-left: 15px;
}


.container-SecondCard{
    padding-left: 30px;
    padding-right: 30px;
    background-color: white;
    margin-top: 40px;
    border-radius: 15px;
}

.container-SecondCard h3 {
    padding-top: 15px;
    padding-bottom: 15px;
}

.progressBar{
    height: 20px;
    width: 230px;
    margin-right: 60px;
    background-color:#eaf1f8;
    align-self: center;
    border-radius:20px
}

.progressTwo{
    height: 20px;
    width: 35px;
    background-color: #FFAB91;
    border-radius:20px  

}
.pointer{
    background-color: white;
    position: absolute;
    height: 20px;
    font-size:15px;

}

.picture{
    width: 20px;
    margin-right: 10px;
    margin-left: 5px;
}
.me{
    display: flex;
    box-shadow:rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;;
    height: 40px;
    width: 180px;
    align-items: center;
    border-radius: 10px;
    margin-right: 10px;
}   






</style>