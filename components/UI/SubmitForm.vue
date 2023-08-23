<template>
  <form class="w-75 align-self-center py-1" @submit.prevent="">
    <input
      class="focus-ring rounded-pill w-100 my-1 p-lg-3 bg-white border-0 custom-placeholder"
      type="text"
      placeholder="E-mail"
    />
    <input
      class="focus-ring rounded-pill w-100 my-2 p-lg-3 bg-white border-0 custom-placeholder"
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
/* Button bg */
button {
  background: transparent linear-gradient(269deg, #2f4fdd 0%, #08377a 100%) 0% 0%
    no-repeat padding-box;
}

/* Input placeholder custom class */
.custom-placeholder::placeholder {
  color: black;
  font-size: 16px;
  font-weight: 500;
}
</style>
