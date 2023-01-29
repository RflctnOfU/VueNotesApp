<template>
  <main>
    <header><h1>Vue Notes App</h1></header>
    <div class="add-note-container">
      <textarea
        name="note"
        id="note"
        cols="30"
        rows="10"
        placeholder="New note"
      ></textarea>
      <button>Add note</button>
    </div>
  </main>
</template>

<style scoped>
main {
  height: 100vh;
  width: 100vw;
}

header {
  padding-top: 5px;
  width: 100%;
  height: 100px;
  text-align: center;
  font-size: x-large;
  font-weight: bold;
  background-color: darkslateblue;
}

.add-note-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 5px 0;
}

.add-note-container button {
  border-radius: 5px 5px;
  cursor: pointer;
  padding: 10px;
  font-size: 17px;
  margin-top: 5px;
  background-color: slateblue;
  color: gainsboro;
}
</style>
