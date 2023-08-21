<template>
  <form class="w-75 align-self-center py-1" @submit.prevent="">
    <input
      class="focus-ring rounded-pill w-100 my-1 p-lg-3"
      type="text"
      placeholder="E-mail"
    />
    <input
      class="focus-ring rounded-pill w-100 my-2 p-lg-3"
      type="text"
      placeholder="Whatsapp"
    />
    <button class="rounded-pill w-100 my-1 btn btn-primary p-lg-3" type="submit">
      Assinar
    </button>
  </form>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
input {
  background-color: #f8f8f8;
  border: 1px solid #d0d0d0;
  border: none;
}

button {
  background: transparent linear-gradient(269deg, #2f4fdd 0%, #08377a 100%) 0% 0%
    no-repeat padding-box;
}
</style>
