<template>
    <div id="table">
        
            <Tableitem v-bind:key="i" v-for="(item,i) in items" v-bind:item="item" v-bind:index="i"/>
    </div>
</template>

<script>
import Tableitem from './Tableitem'
    export default {
        props:'items',
        name:"table",
        components:{
            Tableitem
                }
    }
</script>

<style lang="scss" scoped>

</style>