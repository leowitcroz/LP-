<template>
  <section id="sectionThree">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 3%;
        border-bottom: 2px solid #0077b6;
        background-color: whitesmoke;
      "
    >
      <div class="row">
        <div class="col-lg-6">
          <img
            class="img"
            src="../assets/bro.png"
            alt=""
            style="width: 100%;"
          />
          
        </div>
        <div class="col-lg-6" style="margin-top: 3%;">
          <h1 class="title">TRADUÇÕES & VERSÕES</h1>
          <div class="box">
            <div class="card" v-for="(item, key) in card_texts" :key="key">
              <p class="card-text">
                {{ item.text }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { ref } from "vue";

export default {
  setup() {
    const card_texts = ref([
      {
        text: "Traduções e versões dos idiomas: Português, Inglês e Espanhol",
      },
      {
        text: "Traduções e versão confiáveis, feitas por profissionais com formação, competência e experiência para garantir a adaptabilidade, mas sem perder a fidelidade ao texto original. ",
      },
      {
        text: "Prazo de entrega e qualidade levados muito a sério. Fique tranquilo em relação à qualidade do serviço e prazo de entrega.",
      },
    ]);

    return {
      card_texts,
    };
  },
};
</script>


<style scoped>
.title {
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
  margin-top: 6%;
}

.card {
  padding: 3%;
  background-color: #0077B6;
  margin-top: 5%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  font-size: 20px;
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
  }}
</style>