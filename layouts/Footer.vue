<template>
  <footer>
    <div class="links-footer">
      <h1>loopstudios</h1>
      <div class="link">
        <h3>About</h3>
        <h3>Careers</h3>
        <h3>Events</h3>
        <h3>Products</h3>
        <h3>Support</h3>
      </div>
    </div>
    <div class="social">
      <div class="social-link">
        <fa-icon class="icon" :icon="['fab', 'facebook-square']" />
        <fa-icon class="icon" :icon="['fab', 'twitter-square']" />
        <fa-icon class="icon" :icon="['fab', 'pinterest-square']" />
        <fa-icon class="icon" :icon="['fab', 'instagram-square']" />
      </div>
      <h3>© 2021 Loopstudios. All rights reserved.</h3>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss">
footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 15%;
  background-color: var(--darker);
  height: 25vh;
  width: 100%;
  .links-footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 30%;
    height: 100%;
    margin-left: 12%;
    h1 {
      font-family: "Alita", sans-serif;
      color: var(--light);
    }
    .link {
      display: flex;
      align-items: center;
      justify-content: space-between;
      h3 {
        color: var(--light);
        font-family: "Josefin Sans", sans-serif;
        font-weight: 300;
        cursor: pointer;
        &:hover {
          border-bottom: 2px solid var(--light);
          line-height: 1.5rem;
        }
      }
    }
  }
  .social {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: space-evenly;
    margin-right: 10%;
    .icon {
      font-size: 2rem;
      cursor: pointer;
      margin-left: 0.6rem;
      color: var(--light);
      &:hover {
        border-bottom: 2px solid var(--light);
        line-height: 2rem;
      }
    }
    h3 {
      color: var(--light);
      margin-top: 2rem;
      font-family: "Josefin Sans", sans-serif;
      font-weight: 300;
    }
  }
}
</style>
