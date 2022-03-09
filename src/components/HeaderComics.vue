<template>
  <div class="header-wrapper">
    <div class="header-width">
      <div>
        <img src="../assets/dc-logo.png" alt="">
      </div>

      <ul>
      <li v-for="(link,i) in links" :key="i">
        <a :href="links.href">
          {{ link.text }}
        </a>
      </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComics',
  data() {
    return {
      links: [
    {
    text: "Character",
    href: "#"
    },
    {
      text: "Comics",
      href: "#"
    },
    {
      text: "Movies",
      href: "#"
    },
    {
      text: "Tv",
      href: "#"
    },
    {
      text: "Games",
      href: "#"
    },
    {
      text: "Collectibles",
      href: "#"
    },
    {
      text: "Video",
      href: "#"
    },
    {
      text: "Fan",
      href: "#"
    },
    {
      text: "News",
      href: "#"
    },
    {
      text: "Shop",
      href: "#"
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
* {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  background-color: #fff;

  img {
    
    height: 90%;
  }
}

li {
  height: 100%;
  color: rgb(88, 88, 88);
  text-transform: uppercase;
  font-weight: 800;
  font-size: 12px;
  width: 100px;
  display: flex;
  justify-content: center;

  &:active {
    border-bottom: 3px solid #0C7CEC;
  }
}

.header-wrapper {
  display: flex;
  justify-content: center;
  margin: 0;
}

.header-width {
   width: calc((100% / 12) * 10);
}
</style>
