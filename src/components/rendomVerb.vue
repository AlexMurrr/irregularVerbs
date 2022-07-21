<template>
 
  <formVerbs v-bind:rend=verbForms[rendomNumFromVerbs][0] />
    <div>
       
    </div>
</template>


<script>
import formVerbs from './formVerbsCheck.vue'
export default{

  components:{
    formVerbs
  },

  data(){
    return{
        verbForms: {
            0: ['be', '[быть, являться]', "['was, were']", 'been'],
            1: ['beat', '[бить, колотить]', 'beat', 'beaten'],
            2: ['become', 'становиться', 'became', 'become']
        },
        
    }    
  },
  computed:{
    rendomNumFromVerbs (){
        return Math.floor(Math.random() * Object.keys(this.verbForms).length)
    }
  }

}
</script>


 <style>
 
</style>