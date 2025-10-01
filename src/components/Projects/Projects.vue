<script setup lang="ts">

</script>

<template>
  <div id="projects" class="projects">
    <div class="projects__wrapper">
      <div class="container">
        <div class="projects__content">
          <h2 class="projects__title">Projects</h2>

          <div class="projects__grid">
            <div class="grid-block">
              <div class="grid-block__wrapper">
                <h3 class="grid-block__title">Spicy Play</h3>

                <div class="grid-block__main">
                  <a target="_blank" rel="noreferrer" href="https://spicy-game-seven.vercel.app/" class="grid-block__img">
                  <img src="@/assets/images/projects/spicy_full.jpg" alt="Spicy Game" />
                  </a>

                  <div class="grid-block__list">
                    <h4 class="grid-block__list-title">Tech stack :</h4>

                    <ul class="stack-list">
                      <li class="stack-list__item">Next.js (SSR)</li>

                      <li class="stack-list__item">React</li>

                      <li class="stack-list__item">JavaScript (ES6+)</li>

                      <li class="stack-list__item">SCSS Modules</li>

                      <li class="stack-list__item">next-intl (i18n)</li>

                      <li class="stack-list__item">Semantic HTML</li>
                    </ul>
                  </div>
                </div>

                <div class="grid-block__footer">
                  <a target="_blank" href="https://github.com/Kateryna99/spicy-game" class="grid-block__button button"><span class="icon-github"/> GitHub</a>
                  <a target="_blank" rel="noreferrer" href="https://spicy-game-seven.vercel.app/" class="button button--secondary">
                    Live Demo
                  </a>
                </div>
              </div>
            </div>

            <div class="grid-block">
              <div class="grid-block__wrapper">
                <h3 class="grid-block__title">Spicy Play</h3>

                <div class="grid-block__main">
                  <a target="_blank" rel="noreferrer" href="https://spicy-game-seven.vercel.app/" class="grid-block__img">
                    <img src="@/assets/images/projects/spicy_full.jpg" alt="Spicy Game" />
                  </a>

                  <div class="grid-block__list">
                    <h4 class="grid-block__list-title">Tech stack :</h4>

                    <ul class="stack-list">
                      <li class="stack-list__item">Next.js (SSR)</li>

                      <li class="stack-list__item">React</li>

                      <li class="stack-list__item">JavaScript (ES6+)</li>

                      <li class="stack-list__item">SCSS Modules</li>

                      <li class="stack-list__item">next-intl (i18n)</li>

                      <li class="stack-list__item">Semantic HTML</li>
                    </ul>
                  </div>
                </div>

                <div class="grid-block__footer">
                  <a target="_blank" href="https://github.com/Kateryna99/spicy-game" class="grid-block__button button"><span class="icon-github"/> GitHub</a>
                  <a target="_blank" rel="noreferrer" href="https://spicy-game-seven.vercel.app/" class="button button--secondary">
                    Live Demo
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.projects {
  &__wrapper {
    padding: 40px 0;

    background-color: $dark-forest;
    color: $light-cream;

    @include onTabletAndUp {
      padding: 60px 0;
    }

    @include onLaptopAndUp {
      padding: 80px 0;
    }
  }

  &__content {
    display: flex;
    flex-direction: column;
    gap: 2rem;

    @include onTabletAndUp {
      gap: 3rem;
    }
  }

  &__title {
    @include titleMain;

    color: $terracotta;
  }

  &__grid {
    display: grid;
    grid-template-columns: minmax(200px, 1fr);
    gap: 2rem;

    @include onLaptopAndUp {
      grid-template-columns: repeat(2, minmax(200px, 1fr));
    }
  }
}

.grid-block {
  &__wrapper {
    padding: 1rem;

    display: flex;
    flex-direction: column;
    gap: 1.5rem;

    border-radius: 5px;
    border: 1px solid $sand-beige;

    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1),
    0 1px 3px rgba(0, 0, 0, 0.08);

    @include onTabletAndUp {
      padding: 2rem;
    }
  }

  &__title {
    font-size: $text-24;
    font-weight: $font-weight-bold;
    letter-spacing: 1px;
    text-align: center;

    @include onTabletAndUp {
      font-size: $text-28;
    }
  }

  &__main {
    display: flex;
    flex-direction: column;
    gap: 1rem;

    @include onTabletAndUp {
      gap: 3rem;
    }
  }

  &__img {
    display: block;
    align-self: center;

    max-width: 480px;
    width: 100%;

    height: 50vh;
    max-height: 320px;

    border-radius: 12px;

    overflow: hidden;

    img {
      width: 100%;
      height: 100%;

      object-fit: cover;
      object-position: center;
    }

    @media (min-width: 520px) {
      max-height: 360px;
    }

    @include onTabletAndUp {
      max-width: 520px;

      height: 60vh;
      max-height: 420px;
    }

    @include onDesktopAndUp {
      max-width: 520px;

      height: 70vh;
      max-height: 500px;
    }

    @media (hover: hover) and (pointer: fine) {
      img { display: none; }
      background: url('../../assets/images/projects/spicy_play.png') top center / 100% auto no-repeat;
      transition: background-position 6s linear;

      @include onHover {
        background-position: bottom center;
      }
    }
  }

  &__list {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }

  &__list-title {
    font-weight: $font-weight-bold;
  }

  &__button {
    display: flex;
    align-items: center;
    gap: 5px;
  }

  &__footer {
    display: flex;
    flex-direction: column;
    gap: 1rem;

    @include onTabletAndUp {
      flex-direction: row;
    }
  }
}

.stack-list {
  display: flex;
  flex-direction: column;
  gap: 3px;

  @include onTabletAndUp {
    gap: 5px;
  }

  &__item {
    display: flex;
    align-items: center;
    gap: 5px;

    @include before {
      width: 5px;
      height: 5px;

      border-radius: 50%;
      background-color: $light-cream;
    }
  }
}
</style>
