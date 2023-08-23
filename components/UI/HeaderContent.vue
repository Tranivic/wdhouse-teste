<template>
  <div class="flex-column header-card text-center bg-white mt-5 p-1">
    <img src="../../assets/page_logo.jpg" alt="Page logo" class="page-logo py-2" />
    <div class="card-info py-2">
      <h1 class="my-2 fw- fs-4">Aqui vai um título persuasivo</h1>
      <h2 class="my-2 fs-5">Aqui pode ir uma subheadline mais explicativa</h2>
    </div>
    <div class="form d-flex justify-content-center">
      <UISubmitForm />
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="css" scoped>
/* Font stylization */
h1 {
  font-weight: 900;
}
h1,
h2 {
  color: #152858;
}
</style>
