<template>
 
  <formVerbs 
  :irregularVerb = verbForms[rendomNumFromVerbs][0]
  :translate = verbForms[rendomNumFromVerbs][1]
  :simplePastV = verbForms[rendomNumFromVerbs][2]
  :simpleParticipleV = verbForms[rendomNumFromVerbs][3]
   />
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