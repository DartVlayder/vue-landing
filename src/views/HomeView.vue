<template>
  <div class="container">
    <header class="header">
      <div class="header__left">
        <div class="header__logo">
          <img src="../img/logo.svg" alt="logo">
        </div>
        <nav class="header__menu">
          <button class=" menu__item">
            navitem1
          </button>
          <button class=" menu__item">
            navitem2
          </button>
          <button class=" menu__item">
            navitem3
          </button>
        </nav>
      </div>
      <button class="btn">
        Button
      </button>
    </header>
  </div>

    <main>
      <div class="section__main">
        <div class="bg2"></div>
        <div class="bg1"></div>
        <div class="separator"> </div>
        <h1> Lorem ipsum, dolor sit amet consectetur </h1>

        <div class="section__main__top none">
          <div class="section__main__top--el">
            <img src="../img/headphones.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
          <div class="section__main__top--el">
            <img src="../img/box.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
        </div>

        <div class="section__main__center">
          <div class="section__main__top--el none">
            <img src="../img/laptop.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
          <div class="section__main__top--el">
            <div class="center--img">
              <img src="../img/berries.svg" alt="img" id="berries--img">
            </div>
          </div>
          <div class="section__main__top--el none">
            <img src="../img/paperclip.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
        </div>

        <div class="section__main__bottom none">
          <div class="section__main__top--el">
            <img src="../img/headphones.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
          <div class="section__main__top--el">
            <img src="../img/box.svg" alt="img">
            <div class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</div>
          </div>
        </div>
      </div>
    <div class="container">
      <section class="section__info">
        <div class="card__reviews">
          <div class="separator"></div>
          <h2 class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</h2>
          <div class="card__reviews__comp">
            <div class="card__reviews__comp__avatar">
              <img src="../img/avatar.svg" alt="avatar">
            </div>
            <div class="marks"></div>
            <div class="marks"></div>
            <div class="card__reviews__comp__col">
              <div class="card__reviews__comp__text ">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam quas, aut consectetur
                animi  autem aliquid consequuntur suscipit exercitationem laborum cupiditate magnam eaque quae deleniti, iste nisi
                expedita, provident excepturi officia!
                Porro ab rerum omnis magnam eligendi error nobis dolore? Porro ab rerum omnis magnam eligendi error nobis dolore? Porro ab rerum omnis magnam eligendi error nobis dolore?
              </div>
              <div class="card__reviews__comp__bot">
                <span>Jane Does</span>
                <div class="mark">
                  <div class="marks--bot"></div>
                  <div class="marks--bot"></div>
                </div>
              </div>
            </div>
          </div>

          <div class="card__reviews__df">
            <div class="card__reviews__comp--small">
              <div class="card__reviews__comp--small__text">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam quas, aut consectetur
                animi  autem aliquid
                <div class="name">
                  <span>Jane Does</span>
                </div>
              </div>
              <div class="card__reviews__comp--small__avatar">
                <img src="../img/avatar.svg" alt="avatar">
              </div>
            </div>

            <div class="card__reviews__comp--small">
              <div class="card__reviews__comp--small__avatar">
                <img src="../img/avatar.svg" alt="avatar">
              </div>
              <div class="card__reviews__comp--small__text">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam quas, aut consectetur
                animi  autem aliquid
                <div class="name">
                  <span>Jane Does</span>
                </div>
              </div>
            </div>
            
          </div>

        </div>
        <div class="card__reviews pad-50">
          <div class="separator"></div>
          <div class="reviews__header center">
            <h2>Lorem ipsum, dolor sit 
              adipisicing elit.
            </h2>
            <small>
              Porro ab rerum omnis magnam eligendi error nobis dolore?
            </small>
          </div>
          <div class="accordeon">
            <app-accordeon 
              v-for="(item, index) in items"
              :key="index"
              :image="item.image"
              @click="open(item)"
              :class="{ 'active': item.open === true}"
            ></app-accordeon>
          </div>

        </div>
      </section>
    </div>
    </main>
</template>

<script>
import AppAccordeon from '../components/AppAccordeon.vue'
export default {
  components: {AppAccordeon},
  methods: {
    close () {
      let openItem = this.items.find(item => item.open)
      if (openItem !== undefined) {
        openItem.open = false
      }
    },
    open (item) {
      this.close()
      item.open = !item.open
    }
  },
  data() {
    return {  
      items: [
        {
          image: "el1.svg",
          open: false
        },
        {
          image: "el2.svg",
          open: false
        },
        {
          image: "el3.svg",
          open: false
        },
        {
          image: "el4.svg",
          open: false
        },
        {
          image: "el5.svg",
          open: false
        }
      ]
    }
  },
}
</script>

<style src="./HomeView.scss" lang="scss" scoped>
</style>