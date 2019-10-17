<template>
  <div>
    <table>
      <tr>
        <th>Frutas</th>
        <th>Já adicionou no carrinho?</th>
      </tr>
      <tr v-for="(fruit,index) in fruits" :key="index">
        <td>{{ fruit.name }} </td>
        <td>{{ fruit.completed ? 'SIM' : 'NÃO'}} </td>
        <!-- <td v-if="fruit.completed"> SIM </td>
        <td v-else> NÃO </td> -->
      </tr>
    </table>

  </div>
</template>

<script>
export default {
  data () {
    return {
      fruits: [
        {name: 'Abacaxi', completed: true},
        {name: 'Limão', completed: false},
        {name: 'Manga', completed: true},
        {name: 'Acerola', completed: false},
        {name: 'Uva', completed: true}
      ]
    }
  }
}
</script>
