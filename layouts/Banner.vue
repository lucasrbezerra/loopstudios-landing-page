<template>
  <div class="content">
    <header class="nav">
      <h2 class="logo">loopstudios</h2>
      <div class="links-content">
        <h3 class="links">About</h3>
        <h3 class="links">Careers</h3>
        <h3 class="links">Events</h3>
        <h3 class="links">Products</h3>
        <h3 class="links">Support</h3>
      </div>
    </header>
    <main class="banner">
      <div class="banner-content">
        <h1 class="title">
          IMMERSIVE <br />
          EXPERIENCES <br />
          THAT DELIVER <br />
        </h1>
      </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 100vh;
  background: url("~/assets/images/image-hero.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  .nav {
    height: 20vh;
    width: 75%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: var(--light);
    .logo {
      font-family: "Avala", sans-serif;
      font-size: 1.8rem;
      font-weight: bold;
    }
    .links-content {
      width: 50%;
      display: flex;
      align-items: center;
      justify-content: space-evenly;
      font-family: "Josefin Sans", sans-serif;
      .links {
        cursor: pointer;
        &:hover {
          border-bottom: 2px solid var(--light);
          line-height: 2rem;
        }
      }
    }
  }
  .banner {
    height: 80vh;
    width: 75%;
    display: flex;
    align-items: center;
    .banner-content {
      border: 2px solid var(--light);
      padding: 0.5rem 4rem;
      .title {
        position: relative;
        left: -10%;
        font-family: "Josefin Sans", sans-serif;
        font-size: 3.5rem;
        font-weight: 300;
        line-height: 4.5rem;
        color: var(--light);
        letter-spacing: 0.5rem;
      }
    }
  }
}
</style>
