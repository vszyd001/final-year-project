<template>
  <div class="about">
    <div class="bg-amber-100">
      <InfoQuestion />
    </div>
    <div class="relative">
      <img
        class="w-full"
        src="../assets/creambackground.png"
        alt="Cream illustration background with three people."
      />
      <div class="absolute bottom-20 left-40 text-6xl text-black p-20">
        <h1>Inclusive design</h1>
        <p class="text-2xl">for everyone</p>
      </div>
    </div>

    <div class="text-white p-20 bg-orange-600 text-2xl text-left">
      <img
        class="rounded-full float-right max-h-52 mx-20 my-28 shadow-xl"
        src="../assets/exclamationmark.png"
        alt="Exclamation Mark illustration"
      />
      <!-- start of main section, semantic tags -->
      <main>
        <article>
          <h1 class="text-5xl py-1 px-20">FACTS</h1>
          <p class="m-10">
            People in an age group 65 and above every 2 in 5 people has a
            disability [26].
          </p>
        </article>
        <article>
          <p class="m-10">
            According to World Health Organisation (WHO) 15% of population is
            estimated to experience disability [1].
          </p>
        </article>
        <article>
          <p class="m-10">
            There are 3 types of disabilities: permanent, temporary and
            situational [11].
          </p>
        </article>
      </main>
      <aside>
        <h3 class="m-10 text-xl text-right text-black">
          read more facts below >>
        </h3>
      </aside>
      <!-- Facts clickable buttons -->
      <FactsClick />
    </div>
  </div>
</template>

<script>
import FactsClick from "../components/FactsClick.vue";
import InfoQuestion from "../components/InfoQuestion.vue";

export default {
  name: "AboutView",
  components: {
    InfoQuestion,
    FactsClick,
  },
};
</script>
