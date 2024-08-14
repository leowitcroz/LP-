<template>
  <section id="sectionTwo">
    <div class="container-fluid" style="padding: 0%">
      <div style="background-color: #0077b6; padding: 5%">
        <div class="row">
          <div class="section">
            <h2 class="title">O que você vai aprender</h2>
            <div class="boxes">
              <div
                class="card col-lg-4"
                v-for="(item, key) in card_texts"
                :key="key"
                style="width: 27%; padding: 10px; background-color: #8e44ad; color: whitesmoke; font-size: 18px;"
              >
                <div class="card-body">
                  <p class="card-text">{{ item.text }}</p>
                </div>
              </div>
            </div>
            <button class="btn">Quero começar agora</button>
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
  