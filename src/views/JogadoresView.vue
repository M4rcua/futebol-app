<script>
export default {
  data() {
    return {
      jogadores: [
        { id: 1, nome: "Jogador1" },
        { id: 2, nome: "Jogador2" },
        { id: 3, nome: "Jogador3" },
      ],
    };
  },
};
</script>

<template>
  <h1></h1>
  <div class="container">
    <div class="title">
      <h2>Jogadores</h2>
    </div>
  </div>

  <div class="form-input">
    <input type="text" />
    <button>Salvar</button>
  </div>
  <div class="form-input">
    <input type="text" />
    <button>Salvar</button>
  </div>

  <div class="list-jogadores">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Ações</th>
        </tr>
      </thead>

      <tbody>
        <tr v-for="jogador in jogadores" :key="jogador.id">
          <td>{{ jogador.id }}</td>
          <td>{{ jogador.nome }}</td>
          <td>Posição</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style>
.title {
  text-align: center;
  margin: 2rem 0;
}
.form-input {
  display: flex;
  justify-content: center;
  margin: 2rem 0;
}

.form-input input {
  width: 50%;
  padding: 0.5rem;
  border: 1px solid #ccc;
  border-radius: 10px;
}

.form-input button {
  padding: 0.8rem;
  border: 1px solid rgb(7, 95, 19);
  border-radius: 10px;
  background-color: rgb(20, 172, 0);
  color: white;
  font-weight: bold;
  margin-left: 1%;
}

.list-jogadores {
  display: flex;
  justify-content: center;
}

table {
  width: 50%;
  border-collapse: collapse;
  margin: 0 auto;
  border: 1px solid grey;
  font-size: 1.1rem;
  text-align: center;
}

table thead {
  background-color: rgb(5, 194, 115);
  color: white;
  font-weight: bold;
}

table tbody tr {
  align-items: center;
}

table tbody tr:nth-child(odd) {
  background-color: rgb(213, 228, 250);
}
</style>
