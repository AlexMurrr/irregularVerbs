<template>
    <h1>Изучаем неправильные глаголы</h1>  
    <h2>Введите имя глагола:</h2>
    <h3>{{irregularVerb}} {{translate}} {{simplePastV}} {{simpleParticipleV}}</h3>
    <h3>{{}}</h3>
    <div>
    Translate: &nbsp;&nbsp;
    <input type="text" 
    id="translate" 
    placeholder="перевод" autofocus />
    </div>

    <div>
    Simple Past: &nbsp;&nbsp;
    <input type="text" 
    id="sPast" 
    placeholder="простое прошедшее"/>
    </div>

    <div>
    Simple Participle: &nbsp;&nbsp;
    <input
    type="text"
    id="sParticiple"
    placeholder="простое причастие"/>
    </div>
</template>

<script>
export default{
  props:{
    irregularVerb: String,
    translate: String,
    simplePastV: String,
    simpleParticipleV: String

  } 
}

</script>

<style>
h{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

div{
  font-weight: 400;
  line-height: 1.45;
  font-size: 1.6rem;
  font-weight: 700;
  }
</style>