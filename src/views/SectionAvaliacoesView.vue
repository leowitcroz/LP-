<template>
  <section id="sectionTwo">
    <div
      class="container-fluid"
      style="background-color: whitesmoke; padding: 4%"
    >
      <div class="row" style="display: flex; justify-content: space-around">
        <h1 class="title">DEPOIMENTOS</h1>

        <div
          class="col-lg-12"
          style="display: flex; justify-content: center; margin-bottom: 2%"
        >
          <div class="card">
            <img src="../assets/Dep 2.png" alt="depoimento" />
          </div>
        </div>

        <div
          class="col-lg-12"
          style="display: flex; justify-content: center; margin-bottom: 2%"
        >
          <div class="card">
            <img src="../assets/Dep 3.png" alt="depoimento" />
          </div>
        </div>
        <div
          class="col-lg-12"
          style="display: flex; justify-content: center; margin-bottom: 2%"
        >
          <div class="card">
            <img class="img_" src="../assets/Dep 1.png" alt="depoimento" />
          </div>
        </div>
        <div
          class="col-lg-12"
          style="display: flex; justify-content: center; margin-bottom: 2%"
        >
          <div class="card">
            <img src="../assets/Dep 4.png" alt="depoimento" />
          </div>
        </div>
        <div
          class="col-lg-12"
          style="display: flex; justify-content: center; margin-bottom: 2%"
        >
          <div class="card" >
            <img src="../assets/elogio.jpeg" class="img_" alt="depoimento">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script lang="ts">
import { ref } from "vue";

export default {};
</script>
  
  <style scoped>
.title {
  color: rgb(51, 51, 51);
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  margin-bottom: 4%;
}

.boxes {
  margin-top: 4%;
  display: flex;
  justify-content: space-around;
}

.card {
  padding: 5px;
  background-color: #0077b6;
  color: whitesmoke;
  font-size: 22px;
  width: 50%;
}

.btn {
  margin-top: 3%;
  background-color: #34a853;
  border-radius: 8px;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: Arial;
  font-size: 20px;
  font-weight: bold;
  padding: 13px 32px;
}
.img_ {
  height: 340px;
}
.btn:hover {
  text-decoration: underline;
  background-color: #3ca558;
  color: #ffffff;
}
.btn:active {
  position: relative;
  top: 1px;
}

@media only screen and (max-width: 767px) {
  .title {
    font-size: 1.2rem;
  }

  .card {
    font-size: 13px;
    padding: 5px;
    margin-bottom: 3%;
    width: 100%;
  }


  .btn {
    font-size: 10px;
    margin-bottom: 3%;
  }
  .img_ {
    height: 200px;
  }
}
</style>
  