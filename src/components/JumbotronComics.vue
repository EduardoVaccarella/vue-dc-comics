<template>
  <div>
      <div class="jumbotron-width">
        <h2>
            --> Content goes here
        </h2>
      </div>
  </div>
</template>

<script>
export default {
  name: 'JumbotronComics',
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
* {
    background-color: black;
    display: flex;
    justify-content: center;
    margin-top: 2px;

    .jumbotron-width {
        width: calc((100% / 12) * 10);
        height: 110px;
        display: flex;
        justify-content: flex-start;
        align-items: center;
    }

    h2 {
        color: white;
    }
}
</style>