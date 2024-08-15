<template>
  <section id="sectionTwo">
    <div class="container-fluid" style="padding: 0%">
      <div style="background-color: #0077b6; padding: 5%">
        <div class="row">
          <div class="section">
            <h1 class="title">
              PROGRAMAS DE ACELERAÇÃO & DEMANDAS ESPECÍFICAS
            </h1>
            <div class="boxes">
              <div
                class="card col-lg-4"
                v-for="(item, key) in card_texts"
                :key="key"
                style="
                  width: 27%;
                  padding: 12px;
                  background-color: #8e44ad;
                  color: whitesmoke;
                  font-size: 22px;
                "
              >
                <div
                  class="card-body"
                  style="
                    display: flex;
                    justify-content: center;
                    align-items: center;
                  "
                >
                  <p class="card-text">{{ item.text }}</p>
                </div>
              </div>
            </div>
            <button class="btn">Clique aqui para saber mais</button>
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
        text: " Você precisa dar um UP no seu Inglês em pouco tempo? ",
      },
      {
        text: " Precisa de um HELP específico para uma apresentação, viagem ou entrevista de trabalho?",
      },
      {
        text: " Aqui é onde você encontrará a solução para a sua necessidade atual.",
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
  color: whitesmoke;
  font-weight: 600;
  font-family: Georgia, "Times New Roman", Times, serif;
}

.boxes {
  margin-top: 4%;
  display: flex;
  justify-content: space-around;
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
  text-decoration: none;
  text-shadow: 0px 1px 0px #3d768a;
}
.btn:hover {
  background-color: #3ca558;
  color: #ffffff;
}
.btn:active {
  position: relative;
  top: 1px;
}
</style>
  