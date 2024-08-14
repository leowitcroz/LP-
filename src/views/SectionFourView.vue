<template>
  <section id="sectionFour">
    <div
      class="container-fluid"
      style="
        padding-left: 5%;
        padding-right: 5%;
        padding-top: 3%;
        padding-bottom: 5%;
        background-color: #0077b6;
        padding: 5%;
      "
    >
      <div class="row">
        <div class="col-lg-6" style="display: flex; align-items: center; justify-content: center;flex-direction: column;">
          <h1 class="title">Inglês Específico</h1>
          <div class="card">
              <p class="card-text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate, dolor iste. Quidem qui, animi ad eligendi veniam, temporibus eveniet atque minus at illum eos voluptatibus ratione exercitationem laudantium sed! Perferendis.
              </p>
            </div>
        </div>
        <div class="col-lg-6">
          <img
            src="../assets/image1.png"
            alt=""
            style="width: 100%; margin-top: 10%"
          />
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
  color: whitesmoke;
}

.card {
  padding: 3%;
  background-color: #8e44ad;
  margin-top: 7%;
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  font-size: 22px;
}
</style>