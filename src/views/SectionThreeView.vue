<template>
  <section id="sectionThree">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
      "
    >
      <div class="row">
        <div class="col-lg-6">
          <img
            src="../assets/Pharmacy-Illustration.png"
            alt=""
            style="width: 100%; margin-top: 10%"
          />
        </div>
        <div class="col-lg-6">
          <h1 class="title">Aulas Particulares e Avulsas</h1>
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
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
      },
      {
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
      },
      {
        text: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis facere nam distinctio consequuntur nulla dolor sint sed odio non quia rem molestias at aut repellat, obcaecati mollitia atque, error quos",
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
  background-color: #8e44ad;
  margin-top: 5%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
}
</style>