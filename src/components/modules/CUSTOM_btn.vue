<template>
  <div class="_btn">
    <button>
      {{ text }}
    </button>
  </div>
</template>

<script>
export default {
  name: "CUSTOM_btn",
  props: ["text", "color", "bgColor", "widthPadding", "heightPadding"],
};
</script>

<style lang="scss" scoped>
._btn {
  width: fit-content;
  button {
    color: v-bind(color);
    background-color: v-bind(bgColor);
    padding: v-bind(heightPadding) v-bind(widthPadding);
    border: none;
    outline: none;
    font-size: 24px;
    border-radius: 6px;
  }
}
</style>
