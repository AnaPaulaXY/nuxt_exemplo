<template>
  <div class="container">
    <h1>{{titulo}}</h1>
    <ul>
        <li :key="item.id" v-for = "item in pessoas">
            {{item.nome}} - {{item.idade}} anos
        </li>
    </ul>
    <button>Clique aqui</button>
  </div>
</template>

<script>
export default {
    data: function(){
        return{
            titulo: "Lista de pessoas e idades",
            pessoas: [
                {id: 1, nome: "Marcio", idade: 18},
                {id: 2, nome: "Carla", idade: 16},
                {id: 3, nome: "Lais", idade: 20},
            ]
        }
    }
}
</script>

<style>

</style>