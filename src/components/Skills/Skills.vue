<script setup lang="ts">

</script>

<template>
  <div class="skills">
    <div class="skills__wrapper">
      <div class="container">
        <div class="skills__content">
          <h2 class="skills__title">
            Skills & Tech Stack
          </h2>

          <div class="skills__grid">
            <div class="grid-block">
              <div class="grid-block__wrapper">
                <div class="grid-block__header">
                  <span class="grid-block__icon icon-books"/>
                  <h3 class="grid-block__title">Foundations :</h3>
                </div>

                <ul class="grid-block__list list">
                  <li class="list__item">Semantic HTML</li>
                  <li class="list__item">A11y</li>
                  <li class="list__item">SEO basics</li>
                  <li class="list__item">Web APIs (Fetch, DOM)</li>
                </ul>
              </div>
            </div>

            <div class="grid-block">
              <div class="grid-block__wrapper">
                <div class="grid-block__header">
                  <span class="grid-block__icon icon-paint-format"/>
                  <h3 class="grid-block__title">Styling :</h3>
                </div>

                <ul class="grid-block__list list">
                  <li class="list__item">CSS(SCSS)</li>
                  <li class="list__item">Tailwind</li>
                  <li class="list__item">Vuetify</li>
                </ul>
              </div>
            </div>

            <div class="grid-block">
              <div class="grid-block__wrapper">
                <div class="grid-block__header">
                  <span class="grid-block__icon icon-display"/>
                  <h3 class="grid-block__title">Languages :</h3>
                </div>

                <ul class="grid-block__list list">
                  <li class="list__item">JavaScript</li>
                  <li class="list__item">TypeScript</li>
                </ul>
              </div>
            </div>

            <div class="grid-block">
              <div class="grid-block__wrapper">
                <div class="grid-block__header">
                  <span class="grid-block__icon icon-stack"/>
                  <h3 class="grid-block__title">Frameworks :</h3>
                </div>

                <ul class="grid-block__list list">
                  <li class="list__item">Vue.js (Nuxt)</li>
                  <li class="list__item">React.js (Next)</li>
                </ul>
              </div>
            </div>

            <div class="grid-block">
              <div class="grid-block__wrapper">
                <div class="grid-block__header">
                  <span class="grid-block__icon icon-wrench"/>
                  <h3 class="grid-block__title">Other :</h3>
                </div>

                <ul class="grid-block__list list">
                  <li class="list__item">REST APIs</li>
                  <li class="list__item">Axios</li>
                  <li class="list__item">Git/GitHub</li>
                  <li class="list__item">Docker basics</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.skills {
  &__wrapper {
    padding: 40px 0;

    background-color: $light-cream;

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
  }

  &__grid {
    display: grid;
    grid-template-columns: minmax(200px, 1fr);
    grid-auto-rows: minmax(0, 1fr);
    gap: 1rem;

    @include onTabletAndUp {
      grid-template-columns: repeat(2, minmax(200px, 1fr));
    }

    @include onLaptopAndUp {
      grid-template-columns: repeat(3, minmax(200px, 1fr));
    }
  }
}

.grid-block {
  &__wrapper {
   min-height: 100%;

   padding: 1rem;

   border: 1px solid $dark-forest;
   border-radius: 5px;
  }

  &__header {
    margin-bottom: 1rem;

    display: flex;
    align-items: center;
    gap: 0.7rem;

    font-size: $text-20;
    font-weight: $font-weight-bold;

    @include onTabletAndUp {
      font-size: $text-24;
    }
  }

  &__list {
    display: flex;
    flex-direction: column;
    gap: 5px;
  }
}

.list {
  &__item {
    display: flex;
    align-items: center;
    gap: 5px;

    @include before {
      width: 5px;
      height: 5px;

      border-radius: 50%;
      background-color: $dark-forest;
    }

    @include onTabletAndUp {
      font-size: $text-20;
    }
  }
}

.icon-books {
  color: #E34F26;
}
.icon-paint-format {
  color: #CC6699;
}

.icon-display {
  color: #F7DF1E;
}

.icon-stack {
  color: #61DAFB;
}

.icon-wrench {
  color: #2496ED;
}
</style>
