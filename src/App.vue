<template>
  <div id="app">
    <Navbar :navList="navList" />
    <Main :comics="comics" />
    <Footer :footerList="footerList" />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import comicsJson from './jsons/dc-comics.json'

export default {
  name: 'App',
  components: {
    Navbar,
    Main,
    Footer
  },
  data: function() {
    return {
      comics: comicsJson,
      navList: [
        {
          id: 0,
          name: 'CHARACTERS',
          href: '#'
        },
        {
          id: 1,
          name: 'COMICS',
          href: '#'
        },
        {
          id: 2,
          name: 'MOVIES',
          href: '#'
        },
        {
          id: 3,
          name: 'TV',
          href: '#'
        },
        {
          id: 4,
          name: 'GAMES',
          href: '#'
        },
        {
          id: 5,
          name: 'COLLECTIBLES',
          href: '#'
        },
        {
          id: 6,
          name: 'VIDEOS',
          href: '#'
        },
        {
          id: 7,
          name: 'FANS',
          href: '#'
        },
        {
          id: 8,
          name: 'NEWS',
          href: '#'
        },
        {
          id: 9,
          name: 'SHOP',
          href: '#'
        },
      ],
      footerList: [
        [
          {
            id: 0,
            name: 'DC COMICS',
            href: ''
          },
          {
            id: 1,
            name: 'Characters',
            href: '#'
          },
          {
            id: 2,
            name: 'Comics',
            href: '#'
          },
          {
            id: 3,
            name: 'Movies',
            href: '#'
          },
          {
            id: 4,
            name: 'TV',
            href: '#'
          },
          {
            id: 5,
            name: 'Games',
            href: '#'
          },
          {
            id: 6,
            name: 'Videos',
            href: '#'
          },
          {
            id: 7,
            name: 'News',
            href: '#'
          },
        ],
        [
          {
            id: 0,
            name: 'SHOP',
            href: ''
          },
          {
            id: 1,
            name: 'Shop DC',
            href: '#'
          },
          {
            id: 2,
            name: 'Shop DC Collectibles',
            href: '#'
          },
        ],
        [
          {
            id: 0,
            name: 'DC',
            href: ''
          },
          {
            id: 1,
            name: 'Term Of Use',
            href: '#'
          },
          {
            id: 2,
            name: 'Privacy policy(New)',
            href: '#'
          },
          {
            id: 3,
            name: 'Ad Choices',
            href: '#'
          },
          {
            id: 4,
            name: 'Advertising',
            href: '#'
          },
          {
            id: 5,
            name: 'Jobs',
            href: '#'
          },
          {
            id: 6,
            name: 'Subscriptions',
            href: '#'
          },
          {
            id: 7,
            name: 'Talent Workshops',
            href: '#'
          },
          {
            id: 8,
            name: 'CPSC Certificates',
            href: '#'
          },
          {
            id: 9,
            name: 'Ratings',
            href: '#'
          },
          {
            id: 10,
            name: 'Shop Help',
            href: '#'
          },
          {
            id: 11,
            name: 'Concatc Us',
            href: '#'
          },
        ],
        [
          {
            id: 0,
            name: 'SITES',
            href: '#'
          },
          {
            id: 1,
            name: 'DC',
            href: '#'
          },
          {
            id: 2,
            name: 'MAD Magazine',
            href: '#'
          },
          {
            id: 3,
            name: 'DC Kids',
            href: '#'
          },
          {
            id: 4,
            name: 'DC Universe',
            href: '#'
          },
          {
            id: 5,
            name: 'DC Power Visa',
            href: '#'
          },
        ]
      ]
    }
  }
}
</script>

<style lang="scss">
  @import './style/app.scss';
</style>
