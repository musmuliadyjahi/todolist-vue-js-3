<template>
  <div>
    <input
      class="form-check-input"
      onclick
      type="checkbox"
      value
      id="defaultCheck1"
    />
    <label
      class="form-check-label item"
      v-bind:class="{ 'item-completed': targetSaya.isDone }"
      for="defaultCheck1"
      >{{ targetSaya.namaTarget }}</label
    >
  </div>
</template>

<script>
export default {
  name: "ItemTarget",
  props: ["targetSaya"]
};
</script>

<style scoped></style>
