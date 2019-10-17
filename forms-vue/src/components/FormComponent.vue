<template>
  <div>
    <form>
      <input type="text" placeholder="Nome" v-model="user.name"> {{ user.name }}
      <hr>
      <input type="email" placeholder="E-mail" v-model="user.email"> {{ user.email }}
      <hr>
      <input type="number" placeholder="Idade" v-model="user.age"> {{ user.age }}
      <hr>
      <input type="radio" name="sex" id="fem" value="Fem" v-model="user.sex"> Feminino |
      <input type="radio" name="sex" id="mas" value="Masc" v-model="user.sex"> Masculino
      {{ user.sex }}
      <hr>
      <select v-model="user.state">
        <option value="">Selecione o Estado</option>
        <option value="MS">MS</option>
        <option value="MT">MT</option>
        <option value="SP">SP</option>
      </select> {{ user.state }}
      <hr>
      <label for="agree">Concordo com os termos de uso</label>
      <input type="checkbox" id="agree" v-model="terms"> {{terms}}
      <hr>
      <textarea cols="30" rows="10" v-model="description"></textarea> {{description}}
      <hr>
      <button type="submit"> Enviar </button>
    </form>
  </div>
</template>

<script>
export default {
  data () {
    return {
      user: {
        name: '',
        email: '',
        age: '',
        sex: '',
        state: ''
      },
      terms: true,
      description: ''
    }
  }

}
</script>
