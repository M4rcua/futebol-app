<script>
import { v4 as uuidv4 } from "uuid";
export default {
  data() {
    return {
      times: [
        { id: "9a9223c6-325d-4fb3-9a3d-517832c6f30a", nome: "Time1" },
        { id: "2c05c64c-1c44-43c3-8c2a-db120c5444ec", nome: "Time2" },
        { id: "fe7567c1-49b4-46dc-adc4-0c94a3535924", nome: "Time3" },
      ],
      novo_time: "",
    };
  },
  methods: {
    salvar() {
      const novo_id = uuidv4();
      this.times.push({
        id: novo_id,
        nome: this.novo_time,
      });
    },
  },
};
</script>

<template>
  <h1></h1>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento dos Times</h2>
    </div>
  </div>

  <div class="form-input">
    <input type="text" v-model="novo_time" />
    <button @click="salvar">Salvar</button>
  </div>

  <div class="list-times">
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Nome</th>
          <th>Ações</th>
        </tr>
      </thead>

      <tbody>
        <tr v-for="time in times" :key="time.id">
          <td>{{ time.id }}</td>
          <td>{{ time.nome }}</td>
          <td>???</td>
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
  padding: 0.5rem;
  border: 1px solid rgb(0, 237, 245);
  border-radius: 10px;
  background-color: black;
  color: white;
  font-weight: bold;
  margin-left: 1%;
}

.list-times {
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
