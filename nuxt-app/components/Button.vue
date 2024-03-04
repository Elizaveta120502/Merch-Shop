<template>
<div class="button">
  <div class="button__text">{{text}}</div>
</div>
</template>

<script>
export default {
  name: "Button",
  props:{
    text:{
      type: String,
      default: '',
    }
  }
}
</script>

<style scoped lang="scss">
@import '~/assets/css/_global.scss';
@import '~/assets/css/_variables.scss';
.button{
  background-color: $green;
  width: 100px;
  padding: 8px;
  margin: auto;
  border-radius: 12px;
  font-size: 12px;
  position: absolute;
  top: 300px;
  left: 50%;
  transform:translate(-50%, -50%);
  @include media($sm){
    font-size: 14px;
    top: 450px;
    left: 50%;
  }
  @include media($lg){
    font-size: 16px;
    top: 600px;
    left: 50%;
  }
}

.button__text{
  color: $white;
  font-size: 12px;
  text-align: center;
  @include media($sm){
    font-size: 14px;
  }
  @include media($lg){
    font-size: 16px;
  }
}


</style>