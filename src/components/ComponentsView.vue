<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Aqui vamos a ver componentes la proxima
      
    </h3>
    <!-- lsitado de pasos para crear un componente de Vue 3 -->
    <ol>
      <li>Crear un nuevo archivo .vue</li>
      <li>Definir el template con el HTML</li>
      <li>Definir el script con el JavaScript</li>
      <li>Definir el estilo con el CSS</li>
    </ol>
    <h3>Ejemplo de componente basico</h3>
    <pre>
      <code>
        &lt;template&gt;
          &lt;div&gt;
            &lt;h1&gt;Hola Mundo&lt;/h1&gt;
          &lt;/div&gt;
        &lt;/template&gt;
        &lt;script&gt;
          export default {
            name: 'HelloWorld',
          }
        &lt;/script&gt;
        &lt;style scoped&gt;
          h1 {
            color: red;
          }
        &lt;/style&gt;
      </code>
    </pre>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
