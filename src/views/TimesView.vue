<template>
  <main>Times bons</main>

  <div class="container">
    <div class="title">
      <h2>Gerenciamento dos Times</h2>
    </div>
  </div>

  <div class="form-input">
    <input type="text" />
    <button>Salvar</button>
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
        <tr>
          <td>1</td>
          <td>Time 1</td>
          <td>alguma coisa</td>
        </tr>
        <tr>
          <td>2</td>
          <td>Time 2</td>
          <td>alguma coisa</td>
        </tr>
        <tr>
          <td>3</td>
          <td>Time 3</td>
          <td>alguma coisa</td>
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
  align-items: center;
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
