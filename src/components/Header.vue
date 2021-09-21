<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="">

        <ul>
            <li v-for='(link, index) in Links' :key="index">
                <a :class="(link.current) ? 'active' : null " href="link.url">
                        {{link.text}}
                </a>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          links: [
              {
                  text: 'CHARACTERS',
                  url: '#',
                  current: false,
              },
              {
                  text: 'COMICS',
                  url: '#',
                  current: true,
              },
              {
                  text: 'MOVIE',
                  url: '#',
                  current: false,
              },
              {
                  text: 'TV',
                  url: '#',
                  current: false,
              },
              {
                  text: 'GAMES',
                  url: '#',
                  current: false,
              },
              {
                  text: 'COLLECTIBLES',
                  url: '#',
                  current: false,
              },
              {
                  text: 'VIDEOS',
                  url: '#',
                  current: false,
              },
              {
                  text: 'FANS',
                  url: '#',
                  current: false,
              },
              {
                  text: 'NEWS',
                  url: '#',
                  current: false,
              },
              {
                  text: 'SHOP',
                  url: '#',
                  current: false,
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">
@import "../style/mood";
@import "../style/mixing";

header {
    height: 125px;
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img {
    max-width: 75%;
    }

    ul {
        list-style: none;
        display: flex;


        li a {
            color: black;
            display: flex;
            padding: 0 10px;
            text-decoration: none;
            font-weight: 600;
            font-size: 10px;

  
            &active {
                color: $primary
            }



  
        }
    }   
}
</style>
