<template>
  <div class="profile">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-6">
          <div class="media text-left">
            <img src="../assets/Mus.jpg" class="user-pic mr-3" />
            <div class="media-body">
              <h5 class="mt-0">{{ firstName }} {{ lastName }}</h5>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Facilis deserunt hic cum excepturi rerum.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
export default {
  name: "profile",
  data: function() {
    return {
      firstName: "Musmuliady",
      lastName: "Jahi"
    };
  },
  components: {}
};
</script>

<style scoped>
.user-pic {
  border-radius: 200%;
  height: 80px;
  width: 80px;
}
</style>
