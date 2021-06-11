<template>
  <div class="about-content">
    <div class="image-content"></div>
    <div class="text-content">
      <h1 class="about-title">
        THE LEADER IN <br />
        INTERACTIVE VR <br />
      </h1>
      <p class="about-text">
        Founded in 2011, Loopstudios has been producing world-class <br />
        virtual reality projects for some of the best companies around the
        <br />
        globe. Our award-winning creations have transformed <br />
        businesss through digital experiences that bind to their brand. <br />
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.about-content {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  overflow: hidden;
  background-color: var(--light);
  .image-content {
    position: relative;
    left: 12.5%;
    width: 45%;
    height: 60%;
    background-image: url("~/assets/images/image-interactive.jpg");
    background-size: cover;
    background-repeat: no-repeat;
  }
  .text-content {
    position: relative;
    top: 20%;
    left: 5%;
    padding: 4rem 2rem;
    background-color: var(--light);
    .about-title {
      text-align: center;
      line-height: 4rem;
      font-size: 3rem;
      letter-spacing: 0.5rem;
      font-weight: 300;
    }
    .about-text {
      font-size: 1.2rem;
      font-family: "Alata", sans-serif;
      color: var(--dark-low);
    }
  }
}
</style>
