<template>
  <header>
    <div class="flex-grow one"></div>
    <h1>Veterinary Medicine Calculator</h1>
    <div class="flex-grow two"></div>
    <nav>
      <router-link id="home-link" :to="{name: 'home'}">Home</router-link> | 
      <router-link id='about-link' :to="{name: 'about'}">About</router-link>
    </nav>
    
  </header>
  <router-view id="router-view"/>
</template>

<script>

</script>

<style scoped>
header {
  display: flex;
  position: fixed;
  left: 0;
  top: 0;
  background-color: var(--white-green);
  width: 100%;
  padding: .5rem 0;
  align-items: baseline;
}

#router-view {
  margin-top: 7rem;
}

.flex-grow {
  flex-grow: 1;
}

.one {
  flex-grow: 1.35
}

h1 {
  text-align: center;
  margin-bottom: .25rem;
  color: var(--black-eerie);
}

nav {
  display: flex;
  justify-content: center;
  width: fit-content;
  font-size: 1.3rem;
  margin-right: 1rem;
  color: var(--green-dark);
}

nav > * {
  padding: .2rem .3rem;
}

#home-link {
  margin-right: 1rem;
}

#about-link {
  margin-left: 1rem;
}

a:hover {
  color: var(--white-green);
  background-color: var(--green);
  border-radius: 3px;
}
</style>
