<script lang="ts">
  const date = new Date(Date.now());
  export let dayTime = date.toLocaleDateString(navigator.language, {
    weekday: "short",
    hour: "numeric",
    minute: "numeric",
    hour12: false,
  });
  // @ts-ignore
  const connection =
    // @ts-ignore
    navigator.connection ||
    // @ts-ignore
    navigator.mozConnection ||
    // @ts-ignore
    navigator.webkitConnection;
  let type = connection.effectiveType.toUpperCase();
</script>

<style>
  .wrapper {
    display: flex;
    flex-direction: row;
    position: absolute;
    top: 0;
    width: 100vw;
    overflow: hidden;
    justify-content: space-between;
    backdrop-filter: blur(10px);
    padding: 0.2em 0;
    background: rgba(0, 0, 0, 0.3);
    cursor: pointer;
  }
  .wrapper div {
    display: flex;
    flex-direction: row;
    font-size: small;
    font-weight: 900;
    margin: 0.2em 0;
  }
  .wrapper div > * {
    margin: 0 0.8em;
  }
  .wrapper div img {
    height: 15px;
    color:white;
  }
    /* todo: make this work */

</style>

<nav class="wrapper">
  <div class="start">
    <img src="/apple.svg" alt="apple icon"/>
    <div>Finder</div>
    <div>File</div>
    <div>Edit</div>
    <div>View</div>
    <div>Go</div>
    <div>Window</div>
    <div>Help</div>
  </div>
  <div class="end">
    <i class="material-icons">volume_up</i>
    <i class="material-icons">bluetooth</i>
    <i class="material-icons">wifi</i>
    <i class="material-icons">search</i>
    <div>{type}</div>
    <div>{dayTime}</div>
  </div>
</nav>
