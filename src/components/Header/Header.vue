<template>
  <header class="header">
    <div class="header__wrapper">
      <div class="container">
          <a href="#" class="logo">
            Kateryna Stelmakhova
          </a>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 10;

  height: 5rem;
  width: 100%;

  color: $light-cream;
  background-color: $dark-forest;

  @include onLaptopAndUp {
    height: 6rem;
  }

  &__wrapper {
   padding: 1rem 0;

   min-height: 100%;

   display: flex;
   align-items: center;

   border-bottom: 2px solid $olive-muted;
  }
}
</style>
