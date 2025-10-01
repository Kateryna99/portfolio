<script setup lang="ts">

</script>

<template>
  <div class="hero">
    <div class="hero__wrapper">
      <div class="container">
        <div class="hero__content">
          <div class="hero__header">
            <h1 class="hero__title">Hi, I'm Kateryna</h1>
            <h3 class="hero__subtitle">Frontend Developer | <span>Vue · React · Next.js </span></h3>
          </div>

          <div class="hero__main">
            <p class="hero__text">I build production-ready web apps and thrive in cross-functional teams.</p>

            <p class="hero__text">Experienced with TypeScript, REST APIs and scalable frontend architectures.</p>
          </div>

          <div class="hero__footer">
            <div class="hero__buttons">
              <a href="mailto:katya.stelmakhova@gmail.com" class="button">Hire me</a>

              <a href="#projects" class="button button--secondary">View projects</a>
            </div>

            <div class="hero__block">
              <a target="_blank" rel="noreferrer" href="https://t.me/kstelmakhova" class="hero__link"><span class="icon-telegram"/></a>
              <a target="_blank" rel="noreferrer" href="https://github.com/Kateryna99" class="hero__link"><span class="icon-github"/></a>
              <a target="_blank" rel="noreferrer" href="https://www.linkedin.com/in/kateryna-stelmakhova/" class="hero__link"><span class="icon-linkedin"/></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hero {
  &__wrapper {
    padding: 120px 0 40px;

    @include onTabletAndUp {
      padding: 140px 0 60px;
    }

    @include onLaptopAndUp {
      padding: 200px 0 100px;
    }
  }

  &__content {
    display: flex;
    flex-direction: column;
    gap: 30px;

    @include onTabletAndUp {
      gap: 40px;
    }

    @include onLaptopAndUp {
      gap: 80px;
    }
  }

  &__header {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;

    @include onLaptopAndUp {
      gap: 2.5rem;
    }
  }

  &__title {
    font-family: "Pacifico", cursive;
    font-size: $text-50;
    color: $dark-forest;
    line-height: 1.1;

    @include onTabletAndUp {
      font-size: $text-64;
    }

    @include onLaptopAndUp {
      letter-spacing: 1px;
      font-size: $text-72;
    }
  }

  &__subtitle {
    display: flex;
    flex-direction: column;
    gap: 6px;

    font-size: $text-22;

    @include onTabletAndUp {
      flex-direction: row;
      gap: 1rem;

      font-size: $text-28;
    }

    @include onLaptopAndUp {
      font-size: $text-32;
    }

    span {
      word-spacing: 1rem;
    }
  }

  &__main {
    display: flex;
    flex-direction: column;
    gap: 5px;

    @include onTabletAndUp {
      gap: 1rem;
    }
  }

  &__footer {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;

    @include onTabletAndUp {
      gap: 4rem;
    }
  }

  &__buttons {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;

    @include onTabletAndUp {
      flex-direction: row;
      gap: 1rem;
    }
  }

  &__block {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 2.5rem;

    @include onTabletAndUp {
      gap: 3rem;
    }

    @include onLaptopAndUp {
      justify-content: start;
    }
  }

  &__link {
    font-size: 2rem;

    @include onTabletAndUp {
      font-size: 2.5rem;
    }
  }
}
</style>
