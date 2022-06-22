<!--demo-01a: Implementing and Adding a Message Feed Page Using Vue Router -->
<template>
  <div>
    <h2>Einzigarte Kleidungsstücke für Sie.</h2>
    <p v-for="(m, i) in messages" :key="i">
      {{ m }}
    </p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      messages: [
        'Kleider machen Menschen!',
        'Du willst deinen Kleiderschrank ein bisschen auffrischen? Dann bist du hier genau richtig. Hier findet jeder etwas, dass Ihm gefällt, darunter einzigartige Kleidungsstücke.',
      ]
    }
  }
}
</script>