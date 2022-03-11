<template>
  <div class="main">
    <div class="footer-width">
          <div class="button">
            Sign-up now!
          </div>

          <div class="socials">
            <div class="follow-us">
              Follow us!
            </div>

            <ul>
              <li v-for="(social,i) in socials" :key="i" class="socials">
                <img :src="'../assets/footer-'+ social + '.png'" :alt="social">
              </li>
            </ul>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'FooterComics',
  data() {
    return {
          socials: [
            'facebook',
            'periscope',
            'pintrest',
            'twitter',
            'youtube'
          ]
        }
    },
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">

.main {
    background-color: rgb(51, 51, 51);
    background-size: cover;
    display: flex;
    justify-content: center;
    width: 100%;
    height: 100px;
    z-index: 1;


    .footer-width {
        width: calc((100% / 12) * 10);
        height: 100%;
        padding: 30px 0px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .button {
          padding: 10px;
          border: 2px solid blue;
          color: white;
          text-transform: uppercase;
          font-size: 19px;
        }

        .socials {
          display: flex;
          justify-content: space-between;
          gap: 20px;
          color: white;
        }

        .follow-us {
          text-transform: uppercase;
          font-size: 19px;
          color: blue;
        }

        ul {
          display: flex;
          justify-content: space-evenly;
          gap: 5px;
        }
    }
}

</style>