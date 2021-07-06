<template>
  <header>
    <div class="container header">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="dc">
      </div>
      <nav>
        <ul>
          <li :class="(link.attivo) ? 'bordo-blu' : ''" v-for="(link,index) in links" :key="index"><a :href="link.indirizzo" :class="(link.attivo) ? 'blu' : 'nero'">{{link.nome.toUpperCase()}}</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
    name : 'Header',
    data() {
      return {
        links : [
          {
            nome : 'caracthers',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'comics',
            attivo : true,
            indirizzo : '#' 
          },          
          {
            nome : 'movies',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'tv',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'games',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'collectibles',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'caracthers',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'video',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'fans',
            attivo : false,
            indirizzo : '#' 
          },
          {
            nome : 'news',
            attivo : false,
            indirizzo : '#' 
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
  @import '../style/commons.scss';
  @import '../style/commons-font.scss';

  .container.header {
    display: flex;
    justify-content: space-between;
    height: 120px;
    padding: 20px 0;

    .logo {
      height: $maxHeight;

      img {
        height: $maxHeight;
      }
    }
    nav {
      height: $maxHeight;
      ul {
        list-style: none;
        height: $maxHeight;
        li {
          display: inline-block;
          height: $maxHeight;
          line-height: 80px;
          padding: 0 10px;

          a {
            text-decoration: none;
            font-size : $fontSmall;
          }
        }
      }
    }
  }

</style>