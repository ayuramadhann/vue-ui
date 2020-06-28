<template>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h2>Username</h2>
        <div>
          <div v-for="myuser in user" v-bind:key="myuser.id" class="user">
            <profileitem v-bind:myuser="myuser" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue';
import "bootstrap/dist/css/bootstrap.css";
import profileitem from "./components/profileitem.vue";

export default {
  name: "app",
  data: function() {
    return {
      user: [
        {
          id: 1,
          username: "ayuramadhan",
          status: false
        },
        {
          id: 2,
          username: "ramadhan",
          status: false
        }
      ]
    };
  },
  components: {
    profileitem
  }
};
</script>

<style scoped>
.item-completed {
  color: aquamarines;
}
</style>
