<template>
  <div id="app">
    <CalculadoraAritmetica />
  </div>
</template>

<script>
import CalculadoraAritmetica from './components/CalculadoraAritmetica.vue';

export default {
  components: {
    CalculadoraAritmetica
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', 'Helvetica', 'Arial', sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background: linear-gradient(135deg, #6dd5ed, #ff758c); /* Gradiente de fundo */
  min-height: 100vh; /* Altura total da viewport */
}

input, select {
  font-size: 22px; /* Tamanho da fonte maior */
  margin: 15px; /* Espaço entre os elementos */
  padding: 15px; /* Espaçamento interno */
  border-radius: 8px; /* Borda arredondada */
  border: none; /* Sem borda */
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1); /* Sombra para dar profundidade */
  background-color: rgba(255, 255, 255, 0.9); /* Cor de fundo com transparência */
}

select {
  font-size: 30px; /* 1.5 vezes o tamanho da fonte original */
  margin: 10px;
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ccc;
  cursor: pointer;
}

p {
  font-size: 30px; /* Tamanho maior da fonte */
  color: #ffffff; /* Cor branca para contraste */
  margin-top: 20px;
  padding: 10px;
  border-radius: 5px;
  background-color: rgba(0, 0, 0, 0.5); /* Fundo escuro com transparência */
}

p:hover {
  transform: scale(1.3);
  transition: transform 0.3s ease-in-out;
  background-color: rgba(0, 0, 0, 0.7); /* Fundo mais escuro ao passar o mouse */
}

button {
  font-size: 20px;
  padding: 10px 20px;
  border-radius: 5px;
  border: none;
  cursor: pointer;
  background-color: #4cd137;
  color: white;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
  transition: background-color 0.3s, box-shadow 0.3s;
}

button:hover {
  background-color: #44bd32;
  box-shadow: 0px 6px 8px rgba(0, 0, 0, 0.3);
}

h1 {
  color: #34495e;
  font-size: 36px;
  margin-bottom: 10px;
}

h3 {
  color: #0a585e8a;
  font-size: 20px;
  margin-bottom: 20px;
  text-align: left;
  padding-left: 5%;
}

</style>


