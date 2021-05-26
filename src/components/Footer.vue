<template>
  <footer>
    <div class="footer__copyright">
      <p footer__copyright> &copy; 2021, CheckMate Africa.</p>
    </div>

    <div class="footer__icons">
      <a href="#" class="footer__icon">
        <img src="@/assets/twitter.svg" alt="checkmate twitter">
      </a>
      <a href="#" class="footer__icon">
        <img src="@/assets/instagram.svg" alt="checkmate instagram">
      </a>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer__icons {
  display: flex;
  align-items: center;
}

.footer__icon {
  display: flex;
  align-items: center;

  margin-left: 1rem;
}
</style>