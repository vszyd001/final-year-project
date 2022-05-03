//Reference:https://sfc.vuejs.org/#eyJBcHAudnVlIjoiPHNjcmlwdD5cbmV4cG9ydCBkZWZhdWx0IHtcbiAgZGF0YSgpIHtcbiAgICByZXR1cm4ge1xuICAgICAgbWVzc2FnZTogJydcbiAgICB9XG4gIH1cbn1cbjwvc2NyaXB0PlxuXG48dGVtcGxhdGU+XG4gIDxwPk1lc3NhZ2UgaXM6IHt7IG1lc3NhZ2UgfX08L3A+XG5cdDxpbnB1dCB2LW1vZGVsPVwibWVzc2FnZVwiIHBsYWNlaG9sZGVyPVwiZWRpdCBtZVwiIC8+XG48L3RlbXBsYXRlPiIsImltcG9ydC1tYXAuanNvbiI6IntcbiAgXCJpbXBvcnRzXCI6IHtcbiAgICBcInZ1ZVwiOiBcImh0dHBzOi8vc2ZjLnZ1ZWpzLm9yZy92dWUucnVudGltZS5lc20tYnJvd3Nlci5qc1wiXG4gIH1cbn0ifQ==
//[31]
<template>
  <h1 class="p-5 rounded-lg">Your search: {{ search }}</h1>
  <br />
  <input
    v-model="search"
    placeholder="to search type here"
    class="bg-white px-10 py-4 text-black"
    input="search"
    id="search"
  />
</template>

<script>
export default {
  data() {
    return {
      search: "",
    };
  },
};
</script>
