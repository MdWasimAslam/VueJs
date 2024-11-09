
<script setup>
import { ref } from 'vue';

  const moviesData = ref([
    {
        "title": "Inception",
        "genre": ["Sci-Fi", "Thriller"],
        "release_year": 2010,
        "director": "Christopher Nolan",
        "rating": 8.8,
        "description": "A thief who steals corporate secrets through the use of dream-sharing technology is given the inverse task of planting an idea into the mind of a CEO."
    },
    {
        "title": "The Shawshank Redemption",
        "genre": ["Drama"],
        "release_year": 1994,
        "director": "Frank Darabont",
        "rating": 9.3,
        "description": "Two imprisoned men bond over several years, finding solace and eventual redemption through acts of common decency."
    },
    {
        "title": "The Dark Knight",
        "genre": ["Action", "Crime", "Drama"],
        "release_year": 2008,
        "director": "Christopher Nolan",
        "rating": 9.0,
        "description": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, Batman must accept one of the greatest psychological and physical tests of his ability to fight injustice."
    },
    {
        "title": "Forrest Gump",
        "genre": ["Drama", "Romance"],
        "release_year": 1994,
        "director": "Robert Zemeckis",
        "rating": 8.8,
        "description": "The presidencies of Kennedy and Johnson, the Vietnam War, the Watergate scandal and other historical events unfold from the perspective of an Alabama man with an IQ of 75."
    },
    {
        "title": "Parasite",
        "genre": ["Comedy", "Drama", "Thriller"],
        "release_year": 2019,
        "director": "Bong Joon Ho",
        "rating": 8.6,
        "description": "Greed and class discrimination threaten the newly formed symbiotic relationship between the wealthy Park family and the destitute Kim clan."
    },
    {
        "title": "Interstellar",
        "genre": ["Adventure", "Drama", "Sci-Fi"],
        "release_year": 2014,
        "director": "Christopher Nolan",
        "rating": 8.6,
        "description": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival."
    },
    {
        "title": "Gladiator",
        "genre": ["Action", "Adventure", "Drama"],
        "release_year": 2000,
        "director": "Ridley Scott",
        "rating": 8.5,
        "description": "A former Roman General sets out to exact vengeance against the corrupt emperor who murdered his family and sent him into slavery."
    },
    {
        "title": "Pulp Fiction",
        "genre": ["Crime", "Drama"],
        "release_year": 1994,
        "director": "Quentin Tarantino",
        "rating": 8.9,
        "description": "The lives of two mob hitmen, a boxer, a gangster and his wife intertwine in four tales of violence and redemption."
    },
    {
        "title": "The Matrix",
        "genre": ["Action", "Sci-Fi"],
        "release_year": 1999,
        "director": "The Wachowskis",
        "rating": 8.7,
        "description": "A computer hacker learns from mysterious rebels about the true nature of his reality and his role in the war against its controllers."
    },
    {
        "title": "The Godfather",
        "genre": ["Crime", "Drama"],
        "release_year": 1972,
        "director": "Francis Ford Coppola",
        "rating": 9.2,
        "description": "The aging patriarch of an organized crime dynasty transfers control of his clandestine empire to his reluctant son."
    }
])
</script>




<template>
  <table v-for="(movie,index) in moviesData" :key="index">
    <li>{{ movie.title }}</li>
  </table>
</template>


<style scoped>
  table{
    border:1px solid grey

  }
</style>
