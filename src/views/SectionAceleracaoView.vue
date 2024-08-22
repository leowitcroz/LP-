<template>
  <section id="sectionTwo">
    <div
      class="container-fluid"
      style="background-color: whitesmoke; padding: 4%"
    >
      <div class="row" style="display: flex; justify-content: space-around">
        <h1 class="title">PROGRAMAS DE ACELERAÇÃO & DEMANDAS ESPECÍFICAS</h1>
        <div class="card col-lg-3">
          <div
            class="card-body"
            style="display: flex; justify-content: center; align-items: center"
          >
            <p class="card-text">
              Você precisa dar um <em>UP</em> no seu Inglês em pouco tempo?
            </p>
          </div>
        </div>
        <div class="card col-lg-3">
          <div
            class="card-body"
            style="display: flex; justify-content: center; align-items: center"
          >
            <p class="card-text">
              Precisa de um <em>HELP</em> específico para uma apresentação,
              viagem ou entrevista de trabalho?
            </p>
          </div>
        </div>
        <div class="card col-lg-3">
          <div
            class="card-body"
            style="display: flex; justify-content: center; align-items: center"
          >
            <p class="card-text">
              Aqui é onde você encontrará a solução para a sua necessidade
              atual.
            </p>
          </div>
        </div>
      </div>
      <button class="btn">Clique aqui para saber mais</button>
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
  padding: 15px;
  background-color: #0077b6;
  color: whitesmoke;
  font-size: 22px;
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
  }

  .img {
    display: none;
  }

  .btn {
    font-size: 10px;
    margin-bottom: 3%;
  }
}
</style>
  