<template>
  <main>
    <header><h1>Vue Notes App</h1></header>
    <div class="add-note-container">
      <textarea
        name="note"
        id="note"
        cols="45"
        rows="5"
        placeholder="New note"
      ></textarea>
      <button>Add note</button>
    </div>
    <div class="note-container">
      <div class="note">
        <div class="note-text">
          <p class="text">note text</p>
          <p class="date">date of post</p>
        </div>
        <button class="delete">delete</button>
      </div>
      <div class="note">
        <div class="note-text">
          <p class="text">note text</p>
          <p class="date">date of post</p>
        </div>
        <button class="delete">delete</button>
      </div>
      <div class="note">
        <div class="note-text">
          <p class="text">note text</p>
          <p class="date">date of post</p>
        </div>
        <button class="delete">delete</button>
      </div>
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

.note-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 90%;
  margin: auto;
}

.note {
  display: flex;
  justify-content: space-between;
  border: 1px solid slategrey;
  padding: 10px;
  margin: 5px auto;
  border-radius: 10px;
  width: 50vw;
}

.note-text {
}
.text {
  font-family: monospace;
  font-size: 20px;
}

.date {
  font-size: 10px;
}
.delete {
  background-color: darkred;
  border: none;
  border-radius: 10%;
  color: slategrey;
  height: 30px;
  align-self: center;
}
</style>
