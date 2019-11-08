<template>
    <div>
        <li>
            <span v-bind:class="{done:item.completed}">
                <input type="checkbox" v-on:change="item.completed=!item.completed">
                    {{item.text1}}
            </span>
        </li>
    </div>
</template>

<script>
    export default {
        props:{
         item:{
             type:Object,
             required: true
         },
         index: Number   
        }
    }
</script>

<style lang="scss" scoped>

</style>