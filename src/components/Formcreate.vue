<template>
    <div id="form">
        <form action="">
        <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#">Account Management</b-navbar-brand>

        </b-navbar>
        </form> 
        <Create/>
            <br>
         <Tablelist/>   
    </div>
    
</template>

<script>
    import Tablelist from './Tablelist'
    import Create from './Create'
    export default {
        name :'form',
        components:{
            Tablelist,Create
        },
        
    }
</script>

<style lang="scss" scoped>

</style>