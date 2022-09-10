//
Reference:https://sfc.vuejs.org/#eyJBcHAudnVlIjoiPHNjcmlwdD5cbmV4cG9ydCBkZWZhdWx0IHtcbiAgbWV0aG9kczoge1xuXHQgIHNheShtZXNzYWdlKSB7XG4gICAgXHRhbGVydChtZXNzYWdlKVxuICBcdH1cblx0fVxufVxuPC9zY3JpcHQ+XG5cbjx0ZW1wbGF0ZT5cblx0PGJ1dHRvbiBAY2xpY2s9XCJzYXkoJ2hpJylcIj5TYXkgaGk8L2J1dHRvbj5cbiAgPGJ1dHRvbiBAY2xpY2s9XCJzYXkoJ3doYXQnKVwiPlNheSB3aGF0PC9idXR0b24+XG48L3RlbXBsYXRlPiIsImltcG9ydC1tYXAuanNvbiI6IntcbiAgXCJpbXBvcnRzXCI6IHtcbiAgICBcInZ1ZVwiOiBcImh0dHBzOi8vc2ZjLnZ1ZWpzLm9yZy92dWUucnVudGltZS5lc20tYnJvd3Nlci5qc1wiXG4gIH1cbn0ifQ==
// [28]
<script>
export default {
  methods: {
    show(message) {
      alert(message);
    },
  },
};
</script>

<template>
  <!-- event handling -->
  <div class="text-right text-white mx-20">
    <button
      v-on:click="
        show(
          'People in age group 65 and above are the group with the highest prevalence of disabilities in United States [27].'
        )
      "
      class="shadow-inner px-8 py-4 m-3 rounded-3xl text-lg bg-gray-700"
    >
      Fact #1
    </button>
    <button
      v-on:click="
        show(
          'More than 1 billion people worldwide suffer from variety of disabilities [1].'
        )
      "
      class="text-lg rounded-3xl px-8 py-4 m-3 bg-gray-700"
    >
      Fact #2
    </button>
    <button
      v-on:click="
        show(
          'Disability does not have to be always visible and noticable at first glance [12].'
        )
      "
      class="px-8 py-4 m-3 rounded-3xl text-lg bg-gray-700"
    >
      Fact #3
    </button>
  </div>
</template>
