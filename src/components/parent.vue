<template>
    <div>
<h1>hello zain</h1>
<h1>{{msg}}</h1>
<child name=""/>
    </div>
</template>

<script>
import child from "./child.vue";
    export default {
        name:'parent',
         props: {
    msg: String
  },
        components:{
            child,
        },
        data() {
    return {
      names: ["Zain", "Numan", "Bilal", "Sufyan", " bhi abdullah"],
    };
  },

    }
</script>

<style lang="scss" scoped>

</style>