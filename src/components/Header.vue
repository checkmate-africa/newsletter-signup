<template>
  <header>
    <div class="logo">
      <img alt="checkmate logo" src="@/assets/logo.svg" />
    </div>

    <div class="cta">
      <Button :title="'Get Early Access'" :size="'large'" />
    </div>
  </header>
</template>

<script>
import Button from '@/components/Button.vue'

export default {
  name: 'header',
  components: {
    Button
  }
}
</script>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.cta {
  @media screen and (max-width: 700px) {
    display: none;
  }
}
</style>
