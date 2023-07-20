<template>
  <div class="cabecalho">
    <router-link to="/"><img src="../assets/IMG/flamengo-removebg-preview.png" alt="" class="logo"></router-link>
  </div>

  <div class="">
    <form class="container-formulario ">
      <h1 class="titulo-formulario">Faça seu login</h1>
     <input type="text" class="input-formulario" placeholder="Email/Usuario">
     <input type="text" class="input-formulario" placeholder="Senha">
     <button class="btn-formulario" @click.prevent="proxPagina">LOGIN</button>
    </form>

  </div>

</template>

<script>
export default {
  name: "LoginComponente",

  methods:{
    proxPagina(){
      this.$router.push("/home")
    }
  }
};

</script>
<style> 
  .cabecalho{
    @apply flex justify-center
  }

  .logo{
    @apply w-40 pt-11 pb-7
  }

  .container-formulario{
    @apply bg-pretocinza w-[35%] h-[48vh] flex gap-6 flex-col justify-center items-center  mx-auto rounded-2xl p-3
  }
  
  .titulo-formulario{
    @apply text-2xl text-white font-bold text-center 
  }

  .input-formulario{
    @apply w-72 py-1.5 px-3 rounded-full 
  }
  
  .btn-formulario{
    @apply bg-redsite w-44 py-1.5 rounded-[4px] font-bold hover:bg-black hover:text-white transition duration-500 transform hover:-translate-y-0.5 hover:scale-100 
  }
</style>