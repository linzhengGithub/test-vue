<template>
  <Layout>
    <Types x="-"/>
    <NumberPad/>
  </Layout>
</template>

<script>
  import Types from '@/components/Money/Types'
  import NumberPad from '@/components/Money/NumberPad'
  export default {
    name: 'Money',
    components: {NumberPad, Types}
  }
</script>

<style lang="scss" scoped>
  .nav-wrapper{
    display: flex;
    flex-direction: column;
    height: 100vh;
  }
  .content{
    flex-grow: 1;
    overflow: auto;
  }
</style>