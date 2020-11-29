<script lang="typescript">
  import Doc from "./components/doc.svelte";
import MenuBar from "./components/MenuBar.svelte";


</script>

<style>
  :global(body) {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
  }
  :global(.material-icons) {
    font-family: "Material Icons";
    font-weight: normal;
    font-style: normal;
    font-size: 15px; /* Preferred icon size */
    display: inline-block;
    line-height: 1;
    text-transform: none;
    letter-spacing: normal;
    word-wrap: normal;
    white-space: nowrap;
    direction: ltr;
    /* Support for all WebKit browsers. */
    -webkit-font-smoothing: antialiased;
    /* Support for Safari and Chrome. */
    text-rendering: optimizeLegibility;

    /* Support for Firefox. */
    -moz-osx-font-smoothing: grayscale;

    /* Support for IE. */
    font-feature-settings: "liga";
  }
  .App {
    text-align: center;
    background: url("/wallpaper.jpg");
    height: 100vh;
    width: 100vw;
    background-size: cover;
  }
</style>

<div class="App">
  <MenuBar />
  <Doc />
</div>
