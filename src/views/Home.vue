<template>
  <div class="home">
    <div class="container">
      <div class="row header mb-5 p-3">
        <div class="col-lg-12">
          <h2>Target saya hari ini?</h2>
        </div>
      </div>
      <div class="row content">
        <div class="col-lg-12">
          <div class="Magang-DOT">
            <div class="row">
              <div
                v-for="targetSaya in target"
                v-bind:key="targetSaya.id"
                class="mb-4 target col-lg-12 text-left"
              >
                <ItemTarget v-bind:targetSaya="targetSaya" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import "bootstrap/dist/css/bootstrap.css";
import ItemTarget from "../components/ItemTarget";
export default {
  name: "home",
  data: function() {
    return {
      target: [
        {
          id: 1,
          namaTarget: "Belajar Vue Master Class",
          isDone: false
        },
        {
          id: 2,
          namaTarget: "Belajar Vue CLI 3",
          isDone: false
        },
        {
          id: 3,
          namaTarget: "Push hasil belajar ke Github",
          isDone: false
        }
      ]
    };
  },
  components: {
    ItemTarget
  }
};
</script>

<style scoped>
.home {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.header {
  background-color: #1abc9c;
}

.header h2 {
  margin: 0;
}

.target .item {
  font-size: 20px;
}

.item-completed {
  color: #1abc9c;
}
</style>
