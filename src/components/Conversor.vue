<template>
  <div class="container">
    <h1 class="container__title">Currency converter</h1>
    <div class="container__group">
      <input type="number" class="container__input" />
      <Select></Select>
    </div>
    <div class="container__group">
      <input type="number" class="container__input" readonly />
      <Select></Select>
    </div>
  </div>
</template>

<script>
import Select from "./Select.vue";

export default {
  name: "Conversor",
  components: {
    Select,
  },
};
</script>

<style scoped lang="scss">
.container {
  display: flex;
  flex-direction: column;
  margin: 2rem auto;
  max-width: 450px;

  &__group {
    display: flex;
    align-items: center;
  }

  &__select,
  &__input {
    border: 1px solid gray;
    border-radius: 2rem;
    height: 3rem;
    margin: 0.7rem;
    width: 100%;
  }

  &__input {
    width: 60%;
  }

  &__select {
    flex: 1;
    height: 3.4rem;
    padding: 0.4rem;
  }
}
</style>
