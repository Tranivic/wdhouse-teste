<template>
  <div class="container-fluid h-100vh text-center pt-5">
    <p>
      Página não encontrada. Redirecionando para a página inicial em
      {{ counter }} segundos...
    </p>
  </div>
</template>

<script setup>
const counter = ref(5);

const redirectToHome = async () => {
  const route = useRouter();
  const intervalId = setInterval(() => {
    counter.value--;
    if (counter.value === 0) {
      clearInterval(intervalId);
      console.log("Redirecionando...");
      route.push("/");
    }
  }, 1000);
};

onMounted(() => {
  redirectToHome();
});
</script>
