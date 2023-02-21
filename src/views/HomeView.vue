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
        <swiper
          :slides-per-view="1"
          :space-between="50"
          @swiper="onSwiper"
          @slideChange="onSlideChange"
          class="slider swiper"
          :modules="modules" 
          :pagination="{ clickable: true }"
          navigation
        >
          <swiper-slide class="slider__item slide">
            <img src="../img/box.svg" alt="img">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </swiper-slide>
          <swiper-slide class="slider__item slide">
            <img src="../img/headphones.svg" alt="img">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </swiper-slide>
          <swiper-slide class="slider__item slide">
            <img src="../img/paperclip.svg" alt="img">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </swiper-slide>
          <swiper-slide class="slider__item slide">
            <img src="../img/laptop.svg" alt="img">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </swiper-slide>
        </swiper>
    <div class="container">
      <section class="section__info">
        <div class="card__reviews">
          <div class="separator"></div>
          <h2 class="center">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</h2>
          <div class="card__reviews__comp">
            <div class="card__reviews__comp__avatar">
              <img src="../img/avatar.svg" alt="avatar">
            </div>
            <div class="marks">
              <img src="../img/marks.svg" alt="icon" class="marks__img">
            </div>
            <div class="marks">
              <img src="../img/marks.svg" alt="icon" class="marks__img">
            </div>
            <div class="card__reviews__comp__col">
              <div class="marks__wrapper">
                <div class="marks__wrapper--img">
                  <img src="../img/avatar.svg" alt="avatar">
                </div>
                <div class="marks__wrapper--right">
                  <div class="marks__tel left-1">
                    <img src="../img/marks__op.svg" alt="icon" class="marks__img">
                  </div>
                  <div class="marks__tel left-2">
                    <img src="../img/marks__op.svg" alt="icon" class="marks__img">
                  </div>
                </div>
                <div class="marks__wrapper--left">
                  <div class="marks__tel left-3">
                    <img src="../img/marks__op.svg" alt="icon" class="marks__img">
                  </div>
                  <div class="marks__tel left-4">
                    <img src="../img/marks__op.svg" alt="icon" class="marks__img">
                  </div>
                </div>
              </div>
              <div class="card__reviews__comp__text ">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam quas, aut consectetur
                animi  autem aliquid consequuntur suscipit exercitationem laborum cupiditate magnam eaque quae deleniti, iste nisi
                expedita, provident excepturi officia!
                Porro ab rerum omnis magnam eligendi error nobis dolore? Porro ab rerum omnis magnam eligendi error nobis dolore? Porro ab rerum omnis magnam eligendi error nobis dolore?
              </div>
              <div class="card__reviews__comp__bot">
                <span>Jane Does</span>
                <div class="mark">
                  <div class="marks--bot">
                    <img src="../img/marks.svg" alt="icon" class="marks__img">
                  </div>
                <div class="marks--bot">
                  <img src="../img/marks.svg" alt="icon" class="marks__img">
                </div>
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
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import { defineComponent } from 'vue'
import { Pagination } from 'swiper'
import 'swiper/css/pagination'
import { Navigation } from 'swiper'
import 'swiper/css/navigation' 
export default {
  components: {AppAccordeon,Swiper,SwiperSlide},
  url: import.meta.url,
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log('slide change');
    };
    return {
      onSwiper,
      onSlideChange,
      modules: [Pagination, Navigation]
    };
  },
  methods: {
    close () {
      let openItem = this.items.find(item => item.open)
      if (openItem !== undefined && openItem === true) {
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
  @import '@/styles/variables.scss';
  @import '@/styles/mixins.scss';
  @import './style.scss';

  .swiper {
    @include swiper-wrapper();
  }

  .slide {
    @include swiper-slide();
  }
</style>