<script>
  /* import CitiesList from './components/CitiesList.vue'
    import CounterButton from './components/CounterButton.vue'
    import HelloWorld from './components/HelloWorld.vue'
  */
  import HeaderComponent from './components/HeaderComponent.vue'
  import FooterComponent from './components/FooterComponent.vue'
  // import HamburgerMenu from './components/HamburgerMenu.vue'
  // import { useProductStore } from './stores/ProductStore.js'
  // useProductStore()

  export default {
    components: {
      //CitiesList,
      //CounterButton,
      // HelloWorld
      HeaderComponent,
      FooterComponent
      // HamburgerMenu
    }
  }
</script>
<style>
  main,
  header {
    max-width: 900px;
    /* margin: 175px auto 0px auto; */
    margin: 0 auto;
  }
</style>
<template>
  <body>
    <!-- <nav>
    <ul>
      <li>
        <RouterLink to="/">Home</RouterLink>
      </li>
      <li>
        <RouterLink to="/about">About</RouterLink>
      </li>
      <li>
        <RouterLink to="/contact">Contact</RouterLink>
      </li>
      <li>
        <RouterLink to="/productgallery">Product Gallery</RouterLink>
      </li>
      <li>
        <RouterLink to="/cart">Cart</RouterLink>
      </li>
    </ul>
  </nav> -->
    <header><HeaderComponent /></header>

    <main>
      <RouterView />
    </main>
    <FooterComponent />
  </body>
</template>
