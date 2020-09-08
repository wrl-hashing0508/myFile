<template>
    <div class="box" v-if="flag">
       <header>
          <h2>{{msg}}</h2>
       </header>
       <main>
          <slot>
            <p>
              {{content}}
            </p>
          </slot>
       </main>
       <footer>
          <ul>
            <li>
              <span>{{res}}</span>
              <button>按钮</button>
            </li>
          </ul>
       </footer>
    </div>
</template>

<script>
export default {
  data(){
    return {

    }
  },
  //接受一波
  props:{
    msg:String,
    content:String,
    flag:Boolean,
    res:Number,
  }
}
</script>

<style>
.box{
  width: 300px;
  height: 300px;
  background:salmon;
}
</style>
