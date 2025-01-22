<script lang="ts">
  import earfGif from './assets/earf.gif';
</script>

<main>
  <div id="space">
    <div class="stars"></div>
    <div class="stars"></div>
    <div class="stars"></div>
    <div class="stars"></div>
    <div class="stars"></div>
  </div>
  <div id="content">
    <h1>Rolando World</h1>
    <img src={earfGif} alt="spinning earth" />
    <a href="https://www.linkedin.com/in/rolandoworld/">@linkedin</a>
    <a href="https://bsky.app/profile/rolando.world">@bluesky</a>
  </div>
</main>

<style>
  main {
    height: 100dvh;
    width: 100dvw;
    position: relative;
  }
  #content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 20px;
    height: 100%;
    position: relative;
    z-index: 1000;
  }
  a {
    font-weight: bold;
    color: blue;
    font-size: 1.5rem;
    background: black;
  }
  h1 {
    padding: 0;
    margin: 0;
    font-size: 2.5rem;
    background: black;
  }

  #space,
  .stars {
    overflow: hidden;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
  }

  .stars {
    background-image: radial-gradient(
        2px 2px at 20px 30px,
        #eee,
        rgba(0, 0, 0, 0)
      ),
      radial-gradient(2px 2px at 40px 70px, #fff, rgba(0, 0, 0, 0)),
      radial-gradient(2px 2px at 50px 160px, #ddd, rgba(0, 0, 0, 0)),
      radial-gradient(2px 2px at 90px 40px, #fff, rgba(0, 0, 0, 0)),
      radial-gradient(2px 2px at 130px 80px, #fff, rgba(0, 0, 0, 0)),
      radial-gradient(2px 2px at 160px 120px, #ddd, rgba(0, 0, 0, 0));
    background-repeat: repeat;
    background-size: 200px 200px;
  }
</style>
