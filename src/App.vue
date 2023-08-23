<script setup>

</script>

<template>
  <h1>Calculadora Aritmética</h1>
  <fieldset class="values">
    <legend><h2>Digite aqui os valores</h2></legend>
    <div class="row">
      <label for="number-x">X:</label>
      <input type="number" name="number-x" id="number-x">
    </div>
    <div class="row">
      <label for="number-y">y:</label>
      <input type="number" name="number-y" id="number-y">
    </div>
  </fieldset>
  <fieldset class="operators">
    <legend><h2>Selecione a operação</h2></legend>
    <select name="operadores" id="operadores">
      <option value="">Selecionar operador</option>
      <option value="soma">Soma</option>
      <option value="subtracao">Subtração</option>
      <option value="multiplicacao">Multiplicação</option>
      <option value="divisao">Divisão</option>
    </select>
  </fieldset>
  <fieldset class="result">
    <legend><h2>Resultado:</h2></legend>
    <div id="resultado"></div>
  </fieldset>
</template>

<style scoped>
 h1, h2 {
  margin-block: 16px;
 }

.values,
.operators,
.result {
  padding: 1rem;
  border-style: dotted;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.row {
  width: 100%;
  margin-bottom: 1rem;
  display: flex;
  justify-content: space-between;
}

label {
  width: 5%;
  font-size: 1.2rem;
  margin-right: 1rem;
}

input {
  width: 95%;
}

select {
  width: 100%;
}

input, select {
  padding: 5px;
}

</style>
