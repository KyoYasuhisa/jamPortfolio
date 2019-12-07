<template>
  <div class="font-main flex flex-wrap justify-around">
    <Header />
    <main class="mt-10 p-2">
      <nuxt />
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header'
export default {
  components: {
    Header
  }
}
</script>

<style>
main {
  width: 550px;
}
.photo {
  min-width: 4rem; 
  min-height: 4rem;
  background-image: url('https://i.ibb.co/ryDMwd4/773ea60e51885bbc73b1f348bde094f5.jpg');
}
button:focus {
  outline: none;
}
</style>
