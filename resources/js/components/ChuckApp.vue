<template>
  <div class="wrapper">
    <h1>Frases de Chuck Norris</h1>
    <ul>
      <li v-for="(joke, index) in chuck" :key="index">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chuck: [
        { value: "Chuck Norris puede saltar en paracaídas al espacio exterior." },
        { value: "El principal producto de Chuck Norris es el dolor." },
        { value: "Chuck Norris no lee libros. Los mira fijamente hasta que obtiene la información que quiere." },
        { value: "El tiempo no espera a nadie. A menos que ese hombre sea Chuck Norris." },
        { value: "Si escribes Chuck Norris en Scrabble, ganas. Para siempre." }
      ]
    };
  }
}
</script>

<style scoped>
.wrapper {
  max-width: 600px;
  margin: 2rem auto;
  padding: 1rem;
  font-family: 'Segoe UI', sans-serif;
}
ul {
  list-style: none;
  padding: 0;
}
li {
  background: #fff;
  border-radius: 10px;
  margin: 1rem 0;
  padding: 1rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}
</style>
