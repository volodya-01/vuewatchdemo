<template>
    <div>
        <input v-model="test.text">
    </div>
</template>
<script>
export default {
    name:"Son2",
    data () {
        return {
            test: {
                text1: '',
                text2: ''
            }
        }
    },
     
    watch:{
        'test.text1': {
            deep: true,
            handler: function (newVal,oldVal){
                // code
            }
        }
    }
}
</script>