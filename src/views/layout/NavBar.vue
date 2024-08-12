<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link" href="#"> <RouterLink to="/">Home</RouterLink></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#"> <RouterLink to="/searchResult">SearchResult</RouterLink></a> 
                </li> 
                <li class="nav-item">
                    <a class="nav-link" href="#">Pricing</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link disabled">Disabled</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
import SearchResult from '../searchResult/SearchResult.vue';
import { RouterLink, RouterView } from 'vue-router'


export default {
    name: 'NavBarVue',
    data() {
        return {

        }
    },
    components: {
        SearchResult

  }

}
</script>

<style></style>