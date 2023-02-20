<template>
    <div class="accordeon__el" >
        <div class="accordeon__left">
            <div class="accordeon__img">
              <img :src='require(`../img/${image}`)' alt="img">
            </div>
            <div class="accordeon__text">
                <div class="accordeon__title">
                    Lorem ipsum, dolor sit amet adipisicing elit.
                </div>
                <small class="content">
                    Laboriosam quas, aut consectetur animi autem aliquid consequuntur suscipit exercitationem laborum cupiditate magnam eaque quae delenit
                </small>
            </div>
        </div>
        <div class="accordeon__arrow">
        <img src="../img/arrow.svg" alt="arrow" class="arrow">
        </div>
    </div>
</template>
<script>
export default {
  props: ['index', 'open', 'image']
}
</script>

<style lang="scss">
.accordeon {
    &__img {
      margin-right: 20px;
      max-width: 30px;
    }
    &__arrow {
      max-width: 20px;
    }
    &__left {
      display: flex;
    }
    &__el {
      small {
        display: none;
      }
    }
    &__el.active {
      small {
        display: block;
      }
      .accordeon__title {
        color: #00C368;
        margin-bottom: 10px;
      }
      .arrow {
        transition: 0.3s;
        transform: rotate(180deg);
      }
    }
    .arrow {
      transition: 0.3s;
    }
}

</style>