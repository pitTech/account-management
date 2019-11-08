<template>
    <div>   
        
            Firstname
            <b-form-input v-model="text1" placeholder="First Name"></b-form-input>
            Lastname
            <b-form-input v-model="text2" placeholder="Last Name"></b-form-input>
            Age
            <b-form-input type="number" v-model="text3" placeholder="Age"></b-form-input>
            Birtday
            <b-form-input  type="date" v-model="text1" placeholder="Email"></b-form-input>
            <br>
            <b-form-select v-model="selected" :options="options"></b-form-select>
            <br>
            <br>
            <b-button variant="danger" type="submit">Add</b-button>
            
    </div>
</template>

<script>

    export default {
        data(){
            return{
                selected: null,
                options: [
                { value: null, text: 'Gender' },
                { value: 'a', text: 'Male' },
                { value: 'b', text: 'Female' },
                
                ]
            }
        }
       
    }
</script>

<style lang="scss" scoped>

</style>