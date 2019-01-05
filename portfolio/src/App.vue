<template>
  <div id="app">
    <div id="wrapper" class="flex flex-col h-screen">
      <div id="content" class="flex-1 container mx-auto py-4 text-center antialiased leading-normal">
        <h1 class="text-grey-darker">Hugo Torzuoli</h1>
        <p class="py-2">Hey ! I am Hugo, a 23 years old developer from France 🇫🇷</p>
        <img class="w-48 h-48 my-2" src="./assets/img/profile.png" alt="Profile Avatar">
        <p>
          I love modern web technologies and work with
          <b class="text-grey-darkest">HTML/CSS</b>,
          <b class="text-grey-darkest">JavaScript</b>,
          <b class="text-grey-darkest">Angular</b> (from AngularJS to Angular 7),
          <b class="text-grey-darkest">VueJS</b>,
          <b class="text-grey-darkest">Node</b>.
        </p>
        <p class="py-2">
          In my free time I do some project on
          <a class="no-underline text-blue-dark" href="https://github.com/HZooly" target="_blank">GitHub</a>,
          help people on <a class="no-underline text-blue-dark" href="https://stackoverflow.com/users/4781975/zooly" target="_blank">StackOverflow</a>
          and post some words on <a class="no-underline text-blue-dark" href="https://dev.to/zooly">Dev Community</a>.
        </p>
        <p class="py-2">
          You can find me on <a class="no-underline text-blue-dark" href="https://twitter.com/__Zooly" target="_blank">Twitter</a>,
          <a class="no-underline text-blue-dark" href="https://www.linkedin.com/in/hugotorzuoli/" target="_blank">LinkedIn</a> and
          <a class="no-underline text-blue-dark" href="https://www.instagram.com/__zooly/" target="_blank">Instagram</a>.
        </p>
      </div>
      <footer class="w-full text-center py-1 border-t text-sm">
        This website has been made with <a class="no-underline text-blue-dark" href="https://vuejs.org/" target="_blank">VueJS</a> and
        <a class="no-underline text-blue-dark" href="https://tailwindcss.com/" target="_blank">TailwindCSS</a> and deployed with
        <a class="no-underline text-blue-dark" href="https://surge.sh/" target="_blank">Surge</a>
      </footer>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app'
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
}
</style>
