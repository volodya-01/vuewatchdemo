<template>
    <div>
       <!--  <input v-model="test.text"> -->
        <input v-model="test.text" placeholder="123456">
        <p>{{test.text}}</p>
    </div>
</template>
   
<script>
export default {
    name:"Son",
    data () {
        return {
            test: {
                text: ''
            }
        }
    },
   
    watch:{
        test: {
            deep: true,
            handler: function (newVal,oldVal){
                console.log('newValue', newVal);
                console.log('oldValue', oldVal.text);
            }
        }
    }
}
</script>