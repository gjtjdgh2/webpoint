<!--
  Vue.component("cart-header", {
        template: `<h1>{{ upperTitle }}</h1>`,
        data: function() {
            return {
                title: "Vue Cart"
            }
        },
        computed:{
            //모델이 변경 되면 미리 연산을 수행 ->캐시를 저장해 둔다
            upperTitle: function(){
                return this.title.toUpperCase();
            }
        }
    });
    -->
<template>
    <h1>{{upperTitle}}</h1>
</template>
<script>
export default{
 data: function() {
            return {
                title: "Vue Cart"
            }
        },
        computed:{
            //모델이 변경 되면 미리 연산을 수행 ->캐시를 저장해 둔다
            upperTitle: function(){
                return this.title.toUpperCase();
            }
        }
}
</script>

<style scoped>
h1{
    font-size: 2.0em;
    color:blue;
}

</style>
