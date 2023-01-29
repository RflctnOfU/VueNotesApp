<script setup>
import { ref } from "vue";

const newNote = ref("");
const notes = ref([]);
</script>

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
  /* background-color: darkslateblue; */
  background-image: linear-gradient(to bottom right, darkslateblue, slateblue);
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
  border: none;
  cursor: pointer;
  padding: 10px;
  font-size: 17px;
  margin-top: 5px;
  /* background-color: slateblue; */
  background-image: linear-gradient(to bottom right, darkslateblue, slateblue);
  color: gainsboro;
}
.add-note-container button:hover {
  scale: 105%;
  transition: ease-in-out;
  transition-duration: 0.3s;
}

.add-note-container textarea {
  border-radius: 5px;
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
  background-color: #1d1d1d;
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
  cursor: pointer;
  /* background-color: darkred; */
  background-image: linear-gradient(to bottom right, darkred, red);
  border: none;
  border-radius: 10%;
  color: gainsboro;
  height: 30px;
  align-self: center;
}

.delete:hover {
  scale: 105%;
  transition: ease-in-out;
  transition-duration: 0.3s;
}
</style>
