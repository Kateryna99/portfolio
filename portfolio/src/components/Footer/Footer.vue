<script setup lang="ts">

</script>

<template>
  <footer class="footer">
    <div class="footer__wrapper">
      <div class="container">
        <div class="footer__content">
          <h2 class="footer__title">Contact Me</h2>

          <p class="footer__text">I’m open to new opportunities, collaborations and freelance projects. <span style="font-weight: 700">Feel free to reach out!</span></p>

          <div class="footer__block">
            <a href="mailto:katya.stelmakhova@gmail.com" class="footer__button button button--secondary">Hire me</a>

            <div class="socials">
              <a target="_blank" rel="noreferrer" href="https://t.me/kstelmakhova" class="socials__link"><span class="icon-telegram"/></a>
              <a target="_blank" rel="noreferrer" href="https://github.com/Kateryna99" class="socials__link"><span class="icon-github"/></a>
              <a target="_blank" rel="noreferrer" href="https://www.linkedin.com/in/kateryna-stelmakhova/" class="socials__link"><span class="icon-linkedin"/></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
.footer {
  &__wrapper {
    padding: 20px 0 50px;

    @include onTabletAndUp {
      padding: 40px 0 50px;
    }
  }

  &__content {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  &__title {
    @include titleMain;
    color: $charcoal;
  }

  &__block {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;

    @include onTabletAndUp {
      flex-direction: row;
      justify-content: space-between;
      gap: 2rem;
    }
  }

  &__text {
    max-width: 520px;
    line-height: 1.5;
  }

  &__button {
    @include onTabletAndUp {
      max-width: 240px;
    }
  }
}

.socials {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2rem;

  @include onTabletAndUp {
    justify-content: start;
  }

  &__link {
    font-size: 2rem;

    @include onTabletAndUp {
      font-size: 3rem;
    }
  }
}
</style>
