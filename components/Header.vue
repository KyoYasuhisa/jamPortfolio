<template>
  <header class="md:w-64 w-full h-64 px-2">
    <div class="md:w-64 w-full md:mt-24 mt-12 relative md:fixed">
      <div class="flex">
        <div class="bg-center bg-cover w-16 h-16 mr-2 rounded-full shadow photo"></div>
        <div>
          <h1 class="font-bold">Kyo Yasuhisa</h1>
          <p class="text-xs text-justify">フロントエンドエンジニアのKyo Yasuhisaです。Vue.js, Nuxt.jsが大好きです。Pythonも使います。ご依頼はDMからどうぞ。</p>
        </div>
      </div>
      <div class="flex justify-around mt-5 text-xs">
        <nuxt-link to="/">
          <button>
            <fa icon="code" size="2x" class="block mx-auto mb-1" />
            Works
          </button>
        </nuxt-link>
        <a href="http://" target="_blank" rel="noopener noreferrer">
          <button>
            <fa :icon="['fab','twitter']" size="2x" class="block mx-auto mb-1" />
            Twitter
          </button>
        </a>
        <a href="https://github.com/si-zerodarkthirty" target="_blank" rel="noopener noreferrer">
          <button>
            <fa :icon="['fab','github']" size="2x" class="block mx-auto mb-1" />
            GitHub
          </button>
        </a>
      </div>
      <input type="text" placeholder="Keywords" class="bg-gray-300 p-2 text-xs rounded w-full mt-5 focus:outline-none" v-model="keyword" @keypress.enter="$router.push('/search/'+keyword)">
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      keyword: ''
    }
  }
}
</script>