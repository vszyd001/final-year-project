<template>
  <header>
    <!-- //Reference:https://tailwindcss.com/docs/flex 
    //[34] -->
    <!-- using flexbox for navigation bar -->
    <nav class="flex justify-between bg-gray-600 px-6 py-3 m-0">
      <div class="flex-1 flex-nowrap">
        <!-- navigating between pages -->
        <router-link to="/">
          <img class="max-h-16" src="./assets/logo.png"
        /></router-link>
      </div>
      <router-link to="/" class="flex px-8 pt-4 text-xl">Home</router-link>
      <router-link to="/about" class="flex px-8 pt-4 text-xl"
        >About</router-link
      >
    </nav>
    <router-view />
  </header>

  <!--  footer on the bottom of the page -->
  <footer class="bottom-0">
    <div class="bg-gray-600 py-6 px-6 m-0 absolute bottom w-full">
      <img
        src="./assets/userprofile.jpg"
        class="float-right overflow-hidden h-20 w-20 p-4 rounded-full"
      />
      <div class="absolute m-6 mx-24 px-6">
        <!-- MultiChoice component use -->
        <MultiChoice />
      </div>
      <h1 class="float-right p-7 justify-center">Logged in as Sam</h1>
      <h1 class="float-left py-7 px-1">@2022</h1>
    </div>
  </footer>
</template>

<style lang="scss">
// css applicable to the whole app
#app {
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
  color: white;
  letter-spacing: 0.15em;
}

nav {
  a {
    font-weight: bold;
    color: #ffffff;

    &.router-link-exact-active {
      color: #e7c20d;
    }
  }
}
</style>

<script>
import MultiChoice from "./components/MultiChoice.vue";

export default {
  name: "AboutView",
  components: {
    MultiChoice,
  },
};
</script>
