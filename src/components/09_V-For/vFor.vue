<script setup>
import { ref } from 'vue';

let fruits = ['Apple', 'Mango', 'Banana', 'Guava', 'Oranges'];

let books = ref([
  {
    title: "To Kill a Mockingbird",
    author: "Harper Lee",
    publicationYear: 1960,
    genre: "Fiction",
    ISBN: "978-0060935467"
  },
  {
    title: "1984",
    author: "George Orwell",
    publicationYear: 1949,
    genre: "Dystopian",
    ISBN: "978-0451524935"
  },
  {
    title: "The Great Gatsby",
    author: "F. Scott Fitzgerald",
    publicationYear: 1925,
    genre: "Classic",
    ISBN: "978-0743273565"
  },
  {
    title: "Pride and Prejudice",
    author: "Jane Austen",
    publicationYear: 1813,
    genre: "Romance",
    ISBN: "978-1503290563"
  },
  {
    title: "The Catcher in the Rye",
    author: "J.D. Salinger",
    publicationYear: 1951,
    genre: "Fiction",
    ISBN: "978-0316769488"
  },
  {
    title: "The Hobbit",
    author: "J.R.R. Tolkien",
    publicationYear: 1937,
    genre: "Fantasy",
    ISBN: "978-0547928227"
  }
]);


const movies = ref([
  ["Inception", "The Shawshank Redemption", "The Dark Knight", "Forrest Gump", "The Matrix"],
  ["Pulp Fiction", "Fight Club", "The Godfather", "The Lord of the Rings: The Return of the King", "Interstellar"],
  ["The Empire Strikes Back", "Gladiator", "Titanic", "Braveheart", "Goodfellas"],
  ["Schindler's List", "Se7en", "Saving Private Ryan", "The Silence of the Lambs", "The Green Mile"],
  ["Avatar", "Jurassic Park", "The Lion King", "Back to the Future", "Toy Story"]
])


const gamesData = ref([
  {
    title: "The Legend of Zelda: Breath of the Wild",
    developer: "Nintendo",
    releaseYear: 2017,
    genre: "Action-adventure",
    platforms: ["Nintendo Switch", "Wii U"]
  },
  {
    title: "God of War",
    developer: "Santa Monica Studio",
    releaseYear: 2018,
    genre: "Action-adventure",
    platforms: ["PlayStation 4", "PlayStation 5"]
  },
  {
    title: "Red Dead Redemption 2",
    developer: "Rockstar Games",
    releaseYear: 2018,
    genre: "Action-adventure",
    platforms: ["PlayStation 4", "Xbox One", "PC", "Stadia"]
  },
  {
    title: "Minecraft",
    developer: "Mojang Studios",
    releaseYear: 2011,
    genre: "Sandbox",
    platforms: ["PC", "Mobile", "Console"]
  },
  {
    title: "Fortnite",
    developer: "Epic Games",
    releaseYear: 2017,
    genre: "Battle Royale",
    platforms: ["PC", "PlayStation", "Xbox", "Nintendo Switch", "Mobile"]
  },
  {
    title: "Cyberpunk 2077",
    developer: "CD Projekt",
    releaseYear: 2020,
    genre: "RPG",
    platforms: ["PC", "PlayStation 4", "PlayStation 5", "Xbox One", "Xbox Series X/S"]
  },
  {
    title: "Among Us",
    developer: "InnerSloth",
    releaseYear: 2018,
    genre: "Party",
    platforms: ["PC", "Mobile", "Nintendo Switch", "PlayStation", "Xbox"]
  },
  {
    title: "Overwatch",
    developer: "Blizzard Entertainment",
    releaseYear: 2016,
    genre: "First-person shooter",
    platforms: ["PC", "PlayStation", "Xbox", "Nintendo Switch"]
  },
  {
    title: "Animal Crossing: New Horizons",
    developer: "Nintendo",
    releaseYear: 2020,
    genre: "Simulation",
    platforms: ["Nintendo Switch"]
  },
  {
    title: "Halo Infinite",
    developer: "343 Industries",
    releaseYear: 2021,
    genre: "First-person shooter",
    platforms: ["PC", "Xbox One", "Xbox Series X/S"]
  }
]);



</script>


<template>
  <h1>V-FOR</h1>
  <h2 v-for="(fruit, index) in fruits" :key="index">{{ fruit }}</h2>
  <br>
  <hr>
  <h2 v-for="({ title, author }, index) in books" :key="index">
    <li>Title : {{ title }}</li>
    <li>Author : {{ author }}</li>

  </h2>

  <br>
  <hr>


  <div v-for="(movie, i) in movies" :key="i">
    <div v-for="(singleMovie, j) in movie" :key="j">
      <li>{{ singleMovie }}</li>
    </div>
    <br>
    <hr>
  </div>



  <br>
  <hr>
  <br>

  <!-- Nested forloop -->
  <div v-for="(game, i) in gamesData" :key="i">
    <h4>{{ game }}</h4>
    <div v-for="(property, i) in game" :key="i">
      <li>{{ property }}</li>
    </div>
  </div>

  <!-- simple number iteration -->

  <div v-for="(num, i) in 10" :key="i">
    <p>{{ num }}</p>
  </div>
</template>



<style></style>
