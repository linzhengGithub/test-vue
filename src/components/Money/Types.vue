<template>
  <ul class="types">
    <li :class="type === '-' && 'selected'" @click="selectType('-')">支出</li>
    <li :class="type === '+' && 'selected'" @click="selectType('+')">收入</li>
  </ul>
</template>

<script>
  export default {
    name: "Types",
    props:['x'],
    data(){
      return{
        type:'-' | '+'
      }
    },
    mounted(){
      this.type = this.x
    },
    methods:{
      selectType(type){
        this.type = type
      }
    }
  }
</script>

<style lang="scss" scoped>
  .types{
    display: flex;
    background: #c4c4c4;
    text-align: center;
    > li{
      width: 50%;
      height: 64px;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      &.selected::after{
        content: '';
        position: absolute;
        height: 4px;
        width: 100%;
        bottom: 0;
        left: 0;
        background: black;
      }
    }
  }
</style>