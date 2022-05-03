//Reference:https://michaelnthiessen.com/hover-in-vue/ //[29]
<template>
  <div class="p-4">
    <!-- mouseover and mouseleave event  -->
    <span @mouseover="hover = true" @mouseleave="hover = false">
      <div
        class="rounded-full bg-slate-600 relative w-16 h-16 text-center hover:scale-125 hover:bg-slate-800"
      >
        <div class="text-4xl absolute top-3 right-5 m-0">?</div>
      </div>
    </span>
    <!-- this part is shown only if hover==true so when the cursor is hovered over the question mark -->
    <div v-if="hover" class="text-black text-xl p-10 absolute left-20 top-20">
      There are 3 types of disabilities: permanent, temporary and situational
      [11]. Disability does not have to be visible [12].
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hover: false,
    };
  },
};
</script>
