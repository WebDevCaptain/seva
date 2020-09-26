<script>
  import Nav from '../components/Nav.svelte';
  import Footer from '../components/Footer.svelte';

  export let segment;
</script>

<style>
  main {
    position: relative;
    max-width: 90vw;
    height: 85vh;
    padding: 1rem;
    margin: 0 auto;
    box-sizing: border-box;
    overflow: auto;
  }

  #body {
    background-color: #eee;
  }
</style>

<div id="body">
  <Nav {segment} />

  <main>
    <slot />
  </main>

  <Footer />
</div>
