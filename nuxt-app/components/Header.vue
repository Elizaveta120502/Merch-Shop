<template>
  <div class="header">
<div class="header__inner">
  <div class="header__left">
   <div class="header__left-text">Anne<br>Monner</div>
   <div class="header__left-smile">:)</div>
  </div>
  <div class="header__right">
    <NuxtLink><SvgIcon type="mdi" :path="icons.mdiAccount" class="header__icon"></SvgIcon></NuxtLink>
    <NuxtLink> <SvgIcon type="mdi" :path="icons.mdiCartVariant" class="header__icon"></SvgIcon></NuxtLink>
   <NuxtLink>Доставка</NuxtLink>
   <NuxtLink>Контакты</NuxtLink>
  </div>
</div>
  </div>
</template>

<script>
import { mdiCartVariant, mdiAccount } from '@mdi/js';
import SvgIcon from '@jamescoyle/vue-icon';
export default {
  name: "Header",
  components: {
    SvgIcon,
  },
  data() {
    return {
      icons:{
        mdiCartVariant,
        mdiAccount,
      },
    }
  }
}
</script>

<style scoped lang="scss">
@import '~/assets/css/_global.scss';
@import '~/assets/css/_variables.scss';

.header__inner{
  background-color: $black;
  display: flex;
  justify-content: space-between;
  padding: 10px;
  a {
    color: $white;
    font-size: 12px;
    @include media($sm){
      font-size: 14px;
    }
    @include media($lg){
      font-size: 16px;
    }
  }
}
.header__left{
  display: flex;
  align-items: center;
  gap: 8px;
  margin-right: 15px;
}
.header__left-text{
  color: white;
}

.header__left-smile{
  color: white;
  font-size: 20px;
}
.header__right{
  display: flex;
  gap: 16px;
}

.header__icon{
  color: $white;
}
</style>