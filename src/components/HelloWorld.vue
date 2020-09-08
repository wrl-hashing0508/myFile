<template>
  <div>
    小哥哥  网恋吗？
    <p>
      我还是 个孩子啊
    </p>
    <ul>
      <li v-for="(item,index) in list" :key="index">
          {{item}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data(){
    return{
      list:[1,2,3,5,6,8,9,10],
    }
  }
}
</script>

<style>

</style>