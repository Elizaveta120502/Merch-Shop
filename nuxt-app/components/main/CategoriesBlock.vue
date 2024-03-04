<template>
<div class="categories">
  <div class="categories__inner">
    <div>
    <img src="/assets/images/index/t-shirt.png" class="categories__category"/>
    <div class="categories__text">Футболки и топы</div>
    </div>
    <div>
    <img src="/assets/images/index/socks.png" class="categories__category"/>
    <div class="categories__text">Носки</div>
    </div>
    <div>
      <img src="/assets/images/index/trousers.png" class="categories__category"/>
      <div class="categories__text">Штаны</div>
    </div>
    <div>
      <img src="/assets/images/index/hudi.png" class="categories__category"/>
      <div class="categories__text">Худи</div>
    </div>
    <div>
      <img src="/assets/images/index/shopper.png" class="categories__category"/>
      <div class="categories__text">Сумки и шопперы</div>
    </div>
    <div>
      <img src="/assets/images/index/mug.png" class="categories__category"/>
      <div class="categories__text">Кружки</div>
    </div>
  </div>
</div>
</template>

<script>
import { Carousel, Slide } from 'vue3-carousel';
export default {
  name: "CategoriesBlock",
  components:{
    Carousel,
    Slide,
  }

}
</script>

<style scoped lang="scss">
@import '~/assets/css/_global.scss';
@import '~/assets/css/_variables.scss';

.categories{
  background-color: $white;
  @include media($sm){

  }
  @include media($lg){

  }
}

.categories__inner{
  padding: 20px;
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: space-between;
  @include media($sm){
    width: 90px;
    height: 90px;
  }
  @include media($lg){
    width: 100px;
    height: 100px;
  }
}

.categories__category{
  border-radius: 200px;
  border-color: $black;
  border: solid;
  width: 70px;
  height: 70px;
  padding: 4px;
  @include media($sm){
    width: 90px;
    height: 90px;
  }
  @include media($lg){
    width: 100px;
    height: 100px;
  }
}

.categories__text{
  text-align: center;
  width: 70px;
  font-weight: 300;
  margin: auto;
}


</style>