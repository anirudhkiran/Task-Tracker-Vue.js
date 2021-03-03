<template>
  <button @click="onClick" class="btn" :style="{ background: color }">
    {{ text }}
  </button>
</template>

<script>
// export as default object
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      this.$emit("btn-click");
    },
  },
};
</script>
