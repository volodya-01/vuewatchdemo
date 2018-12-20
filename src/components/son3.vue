<template>
    <div>
        <input v-model="test.text">
    </div>
</template>
<script>
export default {
     name:"Son3",
    data () {
        return {
            test: {
                text1: '',
                text2: ''
            }
        }
    },
    computed:{
        testText1 () {
            return this.test.text1
        }
    },
    watch:{
        testText1: {
            dosomething (newVal,oldVal){
                // code
            }
        }
    }
}
</script>