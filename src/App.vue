<template>
  <div id="app">
    <div id="wrapper" class="flex flex-col h-screen">
      <div id="content" class="flex-1 container mx-auto py-4 text-center antialiased leading-normal">
        <img v-if="$i18n.locale == 'en'" class="float-right w-10 h-10" src="./assets/img/en.svg" @click="switchLang()">
        <img v-if="$i18n.locale == 'fr'" class="float-right w-10 h-10" src="./assets/img/fr.svg" @click="switchLang()">
        <h1 class="text-grey-darker">Hugo Torzuoli</h1>
        <p class="py-2">{{$t("who-am-i")}}</p>
        <img class="w-48 h-48 my-2" src="./assets/img/profile.png" alt="Profile Avatar">
        <p>
          {{$t("technologies")}}
          <span class="text-grey-darkest font-bold">HTML/CSS</span>,
          <span class="text-grey-darkest font-bold">JavaScript</span>,
          <span class="text-grey-darkest font-bold">Angular</span> ({{$t("from")}} AngularJS {{$t("to")}} Angular 7),
          <span class="text-grey-darkest font-bold">VueJS</span>,
          <span class="text-grey-darkest font-bold">Node</span>.
        </p>
        <p class="py-2">
          {{$t("freetime")}}
          <a class="no-underline text-blue-dark" href="https://github.com/HZooly" target="_blank">GitHub</a>,
          {{$t("help")}} <a class="no-underline text-blue-dark" href="https://stackoverflow.com/users/4781975/zooly" target="_blank">StackOverflow</a>
          {{$t("post-words")}} <a class="no-underline text-blue-dark" href="https://dev.to/zooly">Dev Community</a>.
        </p>
        <p class="py-2">
          {{$t("find-me")}} <a class="no-underline text-blue-dark" href="https://twitter.com/__Zooly" target="_blank">Twitter</a>,
          <a class="no-underline text-blue-dark" href="https://www.linkedin.com/in/hugotorzuoli/" target="_blank">LinkedIn</a> {{$t("and")}}
          <a class="no-underline text-blue-dark" href="https://www.instagram.com/__zooly/" target="_blank">Instagram</a>.
        </p>
      </div>
      <footer class="w-full text-center py-1 border-t text-sm">
        {{$t("made-with")}} <a class="no-underline text-blue-dark" href="https://vuejs.org/" target="_blank">VueJS</a> {{$t("and")}}
        <a class="no-underline text-blue-dark" href="https://tailwindcss.com/" target="_blank">TailwindCSS</a> {{$t("deployed")}}
        <a class="no-underline text-blue-dark" href="https://surge.sh/" target="_blank">Surge</a>
        <a class="float-right no-underline text-blue-dark pr-2" href="https://github.com/HZooly/Portfolio" target="_blank">Source</a>
      </footer>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app',
  methods: {
    switchLang: function () {
      switch (this.$i18n.locale) {
        case 'en':
          this.$i18n.locale = 'fr'
          break
        case 'fr':
          this.$i18n.locale = 'en'
          break
        default:
          this.$i18n.locale = 'en'
      }
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
}
</style>
