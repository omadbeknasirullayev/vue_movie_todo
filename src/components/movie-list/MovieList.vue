<template>
    <ul class="movie-list list-goup" >
        <MovieListItem v-for="(movie, index) in movies" :key='index' :movie="movie"/>   
    </ul>
</template>

<script>

    import MovieListItem from "../movie-list-item/MovieListItem.vue"
  

    export default {
        data() {
            return {
                movies: [
                    {name: "Usmon", viewers: 300},
                    {name: "Ertug'rul", viewers: 890},
                    {name: "Hause", viewers: 200},
                    {name: "Jumong", viewers: 789},
                ]
            }
        },
        components: {
            MovieListItem
        },
    }
</script>


<style scoped> 
.movie-list {
    margin-top: 2rem;
    margin-bottom: 1rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px 15px rgba(0, 0, 0, 0.15);
}

</style>