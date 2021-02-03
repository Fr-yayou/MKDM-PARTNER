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
          <div>
              <p>Hello</p>
              <p>Hello</p>
              <p>Hello</p>
          </diV>
      </div>
      <!-- <table class="table">
          <thead>
              <tr>
                  <th>Ressource</th>
                  <th>Current task</th>
                  <th>Actions</th>
              </tr>
          </thead>
          <tbody>
              <tr>
                  <td>Hello</td>
                  <td>Hello</td>
                  <td>Hello</td>
              </tr>
          </tbody>
      </table> -->
  </div>
</template>

<script>
export default {
    name:"Card"
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
/* table{
    width: 100%;
    border-spacing: 0px;
}
table thead tr{
    height: 40px;
    background-color: #eaf1f8;
} */
.table-head{
    display: flex;
    height: 40px;
    background-color: #eaf1f8;
    border-radius: 10px;
    justify-content: space-around;
    align-items: center;
}
.table-head p {
    margin-bottom: 0px;
}
/* table tr:last-child td:first-child {
    border-bottom-left-radius: 10px;
} */
</style>