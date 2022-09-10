<template>
  <!-- search form and text on the background image -->
  <div class="relative">
    <img
      class="w-full"
      src="../assets/yellowbackground.png"
      alt="Yellow illustration background on top of the page. Open book and arrow illustration."
    />
    <!-- //Reference: https://v1.tailwindcss.com/components/forms //[32] -->
    <div class="absolute bottom-20 left-40 text-xl p-20">
      <label for="search" class="text-7xl my-10 text-black"
        >Accessibility</label
      >
      <form class="max-w-lg bottom-0">
        <div class="flex items-center justify-center drop-shadow-lg">
          <SearchForm />
          <button class="bg-gray-600 px-10 py-4">Search</button>
        </div>
      </form>
    </div>
  </div>
  <div
    class="shadow-xl rounded-full relative w-16 h-16 text-center bg-yellow-400 hover:scale-150 hover:bg-yellow-500 float-left m-20"
  >
    <div class="text-4xl text-black absolute top-3 right-6">!</div>
  </div>
  <!-- section 1 -->
  <section>
    <div class="p-20 bg-purple-700 text-white">
      <h1 class="w-full text-4xl text-right px-10 py-4">
        Why is it important?
      </h1>
      <p class="px-10 w-full text-2xl text-right">
        Over 1 billion people worldwide suffer from variety of disabilities [1].
      </p>
    </div>
  </section>
  <!-- section 2 -->
  <section>
    <div class="relative">
      <img
        class="w-full"
        src="../assets/purplebackground.png"
        alt="Purple illustration background. Book and school kit illustration"
      />
      <!-- //Reference:
    https://stackoverflow.com/questions/60362442/cant-center-absolute-position-tailwind-css
    //[33] -->
      <div
        class="absolute w-full transform -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2 text-white"
      >
        <div class="right-44 bottom-0 p-30 absolute max-w-3xl text-left">
          <h1 class="text-6xl p-3">For who?</h1>

          <p class="text-xl">
            Web page focused on accessibility adjustments for people with
            different disabilities like: dyslexia, epilepsy and color blindness.
          </p>
        </div>
        <p></p>
      </div>
    </div>
    <div
      class="rounded-full relative w-16 h-16 text-center bg-gray-700 hover:scale-150 hover:rotate-45 hover:bg-gray-900 float-right m-20"
    >
      <div class="text-4xl absolute top-3 right-5 m-0">✓</div>
    </div>
  </section>
  <!-- section 3 -->
  <section>
    <div class="p-20 bg-amber-50">
      <h1 class="w-full text-4xl text-black text-left px-10">
        Acessibility in web applications
      </h1>
      <p class="px-10 w-full text-2xl text-black text-left">
        It is estimated that 71% of people with access needs will leave a
        website if it is not accessible for them or which they have difficulty
        using [16].
      </p>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
import SearchForm from "../components/SearchForm.vue";

export default {
  name: "HomeView",
  components: {
    SearchForm,
  },
};
</script>
