<template>
  <div class="main">
    <div class="links-width">
          <ul>
            <li v-for="(link,i) in links" :key="i">
                <div v-if="link.title ? 'title' : 'subtitle'">
                    {{ link.text }}
                </div>
            </li>
        </ul>

        <img src="../assets/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>
export default {
  name: 'LinksComics',
  data() {
    return {
        links: [
            {
                text: 'dc comics',
                title: true
            },
            {
                text: 'characters',
                title: false
            },
            {
                text: 'comics',
                title: false
            },
            {
                text: 'tv',
                title: false
            },
            {
                text: 'games',
                title: false
            },
            {
                text: 'videos',
                title: false
            },
            {
                text: 'news',
                title: false
            },
            {
                text: 'shop',
                title: true
            },
            {
                text: 'shop DC',
                title: false
            },
            {
                text: 'shop DC collectibles',
                title: false
            },
            {
                text: 'dc',
                title: true
            },
            {
                text: 'terms of use',
                title: false
            },
            {
                text: 'privacy policy (new)',
                title: false
            },
            {
                text: 'ad choices',
                title: false
            },
            {
                text: 'advertising',
                title: false
            },
            {
                text: 'jobs',
                title: false
            },
            {
                text: 'subscription',
                title: false
            },
            {
                text: 'dc comics',
                title: false
            },
            {
                text: 'characters',
                title: false
            },
            {
                text: 'comics',
                title: false
            },
            {
                text: 'tv',
                title: false
            },
            {
                text: 'games',
                title: false
            },
            {
                text: 'videos',
                title: false
            },
            {
                text: 'news',
                title: false
            },
            {
                text: 'shop',
                title: true
            },
            {
                text: 'shop DC',
                title: false
            },
            {
                text: 'shop DC collectibles',
                title: false
            },
            {
                text: 'dc',
                title: true
            },
            {
                text: 'terms of use',
                title: true
            },
            {
                text: 'privacy policy (new)',
                title: true
            },
            {
                text: 'ad choices',
                title: true
            },
            {
                text: 'advertising',
                title: true
            },
            {
                text: 'jobs',
                title: true
            },
            {
                text: 'subscription',
                title: true
            }
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
    background-image: url('../assets/footer-bg.jpg');
    background-size: cover;
    display: flex;
    justify-content: center;
    height: 500px;
    z-index: -1;

    .links-width {
        width: calc((100% / 12) * 10);
        height: 100%;
        padding: 40px 0px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    ul {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        flex-direction: column;
        flex-wrap: wrap;
        height: 100%;

        li {
            color: white;
            text-transform: capitalize;
            display: flex;
            justify-content: flex-start;
            width: 100%;
            margin-right: 20px;

            .title {
                margin-bottom: 20px;
                font-size: 24px;
            }

            .subtitle {
                color: rgba(0, 0, 0, 0.493);
                font-size: 14px;
            }
        }
    }
}
</style>