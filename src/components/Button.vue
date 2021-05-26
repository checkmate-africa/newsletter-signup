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

    @media screen and (max-width: 1000px) {
      padding: 1rem 3rem;
    }
  }

  &--medium {
    padding: 0.8rem 3rem;

    @media screen and (max-width: 600px) {
      padding: 0.6rem 2rem;
    }

    @media screen and (max-width: 400px) {
      padding: 0.6rem 1.2rem;
    }
  }
  
  &--small {
    padding: 0.5rem 1.5rem;
  }
}
</style>
