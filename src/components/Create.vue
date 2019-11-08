<template>
    <div>   
            <form @submit.prevent="onSubmit">
            Firstname
            <b-form-input type="text" v-model="text1" placeholder="First Name"></b-form-input>
            <br>
            <b-button variant="danger" type="submit">Add</b-button>
            </form>
    </div>
</template>

<script>

    export default {
        data(){
            return{
                texr1:'',
                selected: null,
                options: [
                { value: null, text: 'Gender' },
                { value: 'a', text: 'Male' },
                { value: 'b', text: 'Female' },
                
                ]
            }
        },
        methods:{
            onSubmit(){
                if(this.text1.trim()){
                    const newText1 ={
                        id: Date.now(),
                        text1:this.text1,
                        completed: false
                    }
                    this.$$emit('add-text',newText1)
                    this.text1=""
       
    }
            }
        }
    }  
</script>

<style lang="scss" scoped>

</style>