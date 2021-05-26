<template>
  <button :class="`btn btn--${size}`">
    {{ title }}
  </button>
</template>

<script>
export default {
  name: "button",
  props: {
    title: String,
    size: String,
  },
};
</script>

<style lang="scss" scoped>
.btn {
  padding: 1rem;
  background: var(--col-primary);
  border-radius: 4px;
  border: 1px solid var(--col-primary);
  color: var(--col-white);

  &--large {
    padding: 1rem 5rem;
  }

  &--medium {
    padding: 0.8rem 3rem;
  }
  
  &--small {
    padding: 0.5rem 1.5rem;
  }
}
</style>
