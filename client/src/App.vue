<template>
  <header>
    <nav>
      <router-link id="home-link" :to="{name: 'home'}">Home</router-link> | 
      <router-link id='about-link' :to="{name: 'about'}">About</router-link>
    </nav>
  </header>
  <router-view />
</template>

<script>

</script>

<style scoped>
nav {
  display: flex;
  justify-content: center;
}

#home-link {
  margin-right: 1rem;
}

#about-link {
  margin-left: 1rem;
}
</style>
