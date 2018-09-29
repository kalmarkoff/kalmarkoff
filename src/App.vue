<template>
  <div id="app">
    <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
      <a class="navbar-brand" href="#">Fixed navbar</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"/>
      </button>
      <div id="navbarCollapse" class="collapse navbar-collapse">
        <ul class="navbar-nav mr-auto">
          <router-link to="/" class="nav-item" tag="li">
            <a class="nav-link">Home</a>
          </router-link> |
          <router-link to="/about" class="nav-item" tag="li">
            <a class="nav-link">About</a>
          </router-link>
          <router-link to="/Add" class="nav-item" tag="li">
            <a class="nav-link">Add</a>
          </router-link>
        </ul>
      </div>
    </nav>
    <router-view/>
  </div>
</template>








<style>
#app {
  margin-top: 80px;
}
</style>
