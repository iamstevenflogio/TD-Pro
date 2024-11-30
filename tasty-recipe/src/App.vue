<script>
import HomePage from "./components/pages/HomePage.vue"
import RecipeList from "./components/recipe/RecipeList.vue"

import WebHeader from "./components/header/WebHeader.vue"
import NavigationBar from "./components/header/NavigationBar.vue"
import WebFooter from "./components/footer/WebFooter.vue"
export default {
components: {
HomePage,
RecipeList,
WebHeader,
NavigationBar,
WebFooter
}
}

</script>

<template>
  <header>
    <div>
    <WebHeader />
      <HomePage /> 
      <RecipeList />
    <WebFooter />
  </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>

</style>
