<template>
    <div id="table">
        <b-table striped hover :items="items"  >
            <Tableitem/>
        </b-table>
    </div>
</template>

<script>
import Tableitem from './Tableitem'
    export default {
        name:"table",
         data() {
      return {
        items: [
          { first_name: 'Dickerson', last_name: 'Macdonald', age: 40, Birtday:'11/08/2019', gender:'Male'  },
        ]
      }
    },
    components:{
        Tableitem
    }
    }
</script>

<style lang="scss" scoped>

</style>