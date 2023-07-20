<template>
  <nav class="container-nav">
    <div>
       <router-link to="/"><img src="../assets/IMG/flamengo-removebg-preview.png" alt="" class="logo-nav"></router-link>
    </div>

    <div class="">
      <input type="text" class="input-nav"  placeholder="Pesquisar..."/>
    </div>

    <div class="flex gap-4 ml-72">
      <router-link to=""  class="link-nav">Jogos</router-link>
      <router-link to=""  class="link-nav">Central de ajuda</router-link>
      <router-link to="/" class="link-nav">Entrar/Cadastrar</router-link>
    </div>

    <div class="flex gap-4 ml-48">
      <i class="fa-brands fa-square-facebook text-2xl text-white  hover:text-redsite transition duration-500"></i>
      <i class="fa-brands fa-instagram text-2xl text-white  hover:text-redsite transition duration-500"></i>
      <i class="fa-brands fa-twitter text-2xl text-white  hover:text-redsite transition duration-500"></i>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style>
    .container-nav{
      @apply  bg-pretocinza flex py-2 items-center px-7
    }
    .logo-nav{
        @apply w-16
    }
    .link-nav{
        @apply text-white font-bold hover:text-redsite hover:underline transition duration-500
    }
    .input-nav{
        @apply w-[150%] ml-9 rounded-full px-4 py-1
    }
</style>
