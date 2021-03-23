<template>
  <div>
    <ul>
      <li v-for="fournisseur in fournisseurs" :key="fournisseur.nom">
        {{ fournisseur.nom }} ({{ fournisseur.ville}})
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Fournisseur",
  data() {
    return {
      fournisseurs: [
      { nom: 'Foo', ville:'Troyes' },
      { nom: 'Bar', ville:'Paris' }
    ]}
  }
}
</script>

<style scoped>

</style>
