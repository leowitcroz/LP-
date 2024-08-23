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
          <img class="img" src="../assets/bro.png" alt="" style="width: 100%" />
        </div>
        <div class="col-lg-6" style="margin-top: 3%">
          <h1 class="title">TRADUÇÕES & VERSÕES</h1>
          <div class="box">
            <div class="card" v-for="(item, key) in card_texts" :key="key">
              <p class="card-text">
                {{ item.text }}
              </p>
            </div>
          </div>
          <button class="btn">
            <a
              href="https://wa.me/5511973741976?text=Tenho%20interesse%20em%20orçamento%20de%20tradução/versão"
              >Clique aqui para saber mais</a
            >
          </button>
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

.btn a {
  color: whitesmoke;
  text-decoration: none;
}

.card {
  padding: 3%;
  background-color: #0077b6;
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

  .btn {
    font-size: 10px;
    margin-bottom: 3%;
  }
}
</style>