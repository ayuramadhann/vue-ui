<template>
  <div>
    <input class="form-check-input" type="checkbox" id="defaultCheck1" />
    <label class="mt-1" v-bind:class="{ 'item-completed': myuser.status }">
      {{
      myuser.username
      }}
    </label>
  </div>
</template>

<script>
export default {
  name: "profileitem",
  props: ["myuser"]
};
</script>
<style scoped></style>
