<template>
  <div id="app">
    <div class="container">
      <!-- row header marginbottom-5 dan padding-5 -->
      <div class="row header mb-5 p-5">
        <div class="col-lg-12">
          <h2>What I do Today?</h2>
        </div>
      </div>
      <div class="row content">
        <div class="col-lg-12">
          <div class="pekerjaan-rumah">
            <div class="row">
              <div  v-for="tugasSaya in tugas"
                    v-bind:key="tugasSaya.id" 
                    class="mb-3 tugas col-lg-12 text-left">
                <!-- checkbox -->
               
              </div> 
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'

export default {
  name: "app",
  data: function() {
    return {
      tugas: [
        {
          id: 1,
          namaTugas: "Belanja di Shopee",
          isDone: false
        },
        {
          id: 2,
          namaTugas: "Ngoding",
          isDone: false
        },
        {
          id: 3,
          namaTugas: "Ngegame",
          isDone: false
        },
        {
          id: 4,
          namaTugas: "Ngedesain",
          isDone: false
        },
        {
          id: 5,
          namaTugas: "Ngulik",
          isDone: false
        },
        {
          id: 6,
          namaTugas: "Belajar",
          isDone: false
        },
        {
          id: 1,
          namaTugas: "Buka Puasa",
          isDone: false
        }
      ]
    };
  },
  component: {
    ItemTugas
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialised;
  -mos-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.header{
  background: #1abc9c;
}
.header h2{
  margin: 0;
}
.tugas .item{
  font-size: 20px;
  text-align: left;
}
.item-completed{
  color: green;
}
</style>
