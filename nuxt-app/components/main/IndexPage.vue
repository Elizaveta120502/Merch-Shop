<template>
<div class="main-page">
  <div class="main-page__inner">
     <div class="main-page__first">
       <div class="main-page__border-block">
         <img src="/assets/images/index/logo.png" class="main-page__logo"/>
         <Button text="Погнали !"/>
         <div class="main-page__border-block-text">
           Каждый день - это возможность для роста и развития. Верь в себя! Возможно что угодно!<br>
           Неважно, сколько раз ты споткнулся, важно - сколько раз ты поднялся!
         </div>
       </div>
     </div>
     <div></div>
     <div></div>
  </div>
</div>
</template>

<script>
import Button from "../Button.vue";
export default {
  name: "IndexPage",
  components: {Button}
}
</script>

<style scoped lang="scss">
@import '~/assets/css/_global.scss';
@import '~/assets/css/_variables.scss';
.main-page{

}
.main-page__first{
  background: url('assets/images/index/bg-image.png');
  background-size: cover;
  display: flex;
  justify-content: center;
  height: 400px;
  @include media($sm){
    height: 600px;
  }

  @include media($lg){
    height: 750px;
  }
}

.main-page__logo{
  width: 80%;
  position: absolute;
  top: 200px;
  left: 50%;
  transform:translate(-50%, -50%);
  @include media($sm){
    top: 270px;
    left: 50%;
  }

  @include media($lg){
    top: 400px;
    left: 50%;
  }
}

.main-page__border-block{
  border: solid 2px;
  border-color: $white;
  border-radius: 12px;
  margin: 20px;
  width: 50%;

  .main-page__border-block-text{
    color: $white;
    text-align: center;
    position: absolute;
    top: 370px;
    padding: 12px;
    left: 50%;
    transform:translate(-50%, -50%);
    font-size: 12px;

    @include media($sm){
      font-size: 14px;
      top: 550px;
    }

    @include media($lg){
      font-size: 16px;
      top: 680px;
    }
  }
}


</style>