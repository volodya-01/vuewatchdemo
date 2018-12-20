<template>
  <div class="hello">
   <div class="son">
      <div>使用 Vue 中的 watch 方法监听对象，设置 deep:true 可以进行深度监听，当对象中的属性发生变化时，会调用 handler 方法。</div>
       <Son/>
   </div>
  <div class="son2">
    <div>如果需要只监听对象中某一属性的变化，watch 也能实现，另外也可以结合使用计算属性 computed 来对此进行监听。 </div>
     <Son2/>
  </div>
   <div class="son3">
     <div>以下是结合计算属性对某一对象的单一属性实现监听的方法：</div>
     <Son3/>
   </div>
  </div>
</template>

<script>
import Son from '@/components/son'
import Son2 from '@/components/son2'
import Son3 from '@/components/son3'
export default {
  name: 'HelloWorld',
  components:{
    Son,
    Son2,
    Son3
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.son{
  widows: 50vw;
  height: 10vh;
  border: 1px red dashed;
}
.son2{
  widows: 50vw;
  height: 10vh;
    border: 1px red dashed;
}
.son3{
  widows: 50vw;
  height: 10vh;
    border: 1px red dashed;
}
</style>
