<template>
  <component :is="iconComponent" />
</template>

<script>
const icons = {
  error: require("./Icons/ErrorIcon.vue").default,
  success: require("./Icons/SuccessIcon.vue").default,
  info: require("./Icons/InfoIcon.vue").default,
};

export default {
  name: "BaseIcon",
  props: {
    name: {
      type: String,
      required: true,
      validator(value) {
        return Object.prototype.hasOwnProperty.call(value, icons);
      },
    },
  },
  computed: {
    iconComponent() {
      return icons[this.name];
    },
  },
};
</script>
