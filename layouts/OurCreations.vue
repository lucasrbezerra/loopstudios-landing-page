<template>
  <div class="creations-content">
    <header class="creations-header">
      <h2>OUR CREATIONS</h2>
      <button class="see-all">SEE ALL</button>
    </header>
    <div class="cards">
      <div v-for="(photo, index) of photos" :key="index" class="card-content">
        <img :src="`${require(`~/assets/images/creations/${photo.image}`)}`" />
        <h3>{{ photo.text }}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    photo: "image-curiosity.jpg",
    photos: [
      { image: "image-curiosity.jpg", text: "THE CURIOSITY" },
      { image: "image-deep-earth.jpg", text: "DEEP EARTH" },
      { image: "image-fisheye.jpg", text: "MAKE IT FISHEYE" },
      { image: "image-from-above.jpg", text: "FROM UP ABOVE VR" },
      { image: "image-grid.jpg", text: "THE GRID" },
      { image: "image-night-arcade.jpg", text: "NIGHT ARCADE" },
      { image: "image-pocket-borealis.jpg", text: "POCKET BOREALIS" },
      { image: "image-soccer-team.jpg", text: "SOCCER TEAM VR" },
    ],
  }),
};
</script>

<style lang="scss">
.creations-content {
  background-color: var(--light);
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 100vh;
  .creations-header {
    display: flex;
    align-items: center;
    width: 75%;
    justify-content: space-between;
    h2 {
      color: var(--dark);
      font-size: 1.6rem;
      font-weight: 400;
      letter-spacing: 0.3rem;
    }
    button {
      width: 12%;
      height: 50%;
      color: var(--light);
      background-color: var(--dark);
      border: none;
      outline: none;
      cursor: pointer;
      &:hover {
        background-color: var(--darker);
      }
    }
  }
  .cards {
    display: grid;
    grid-template-columns: 25% 25% 25% 25%;
    grid-template-rows: 48% 48%;
    align-items: center;
    gap: 10px;
    width: 75%;
    height: 100%;
    margin-bottom: 10px;
    .card-content {
      height: 100%;
      width: 100%;
      img {
        height: 100%;
        width: 100%;
        cursor: pointer;
      }
      h3 {
        width: 75%;
        position: relative;
        top: -40%;
        left: 5%;
        font-size: 1.5rem;
        font-family: "Josefin Sans", sans-serif;
        color: var(--light);
        line-height: 2.3rem;
        letter-spacing: 0.5rem;
      }
      &:hover{
        img {
          opacity: 0.5;
        }
        h3 {
          color: var(--darker);
        }

      }
    }
  }
}
</style>