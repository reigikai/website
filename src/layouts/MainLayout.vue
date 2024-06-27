<template>
  <q-layout view="hHh lpR fFf">

    <q-header reveal bordered class="bg-primary text-black" height-hint="98">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

      </q-toolbar>

    </q-header>
    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
    >
      <q-list>
        <q-item-label
          header
        >
          Explore below
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
  import { defineComponent, ref } from 'vue'
  import EssentialLink from 'components/EssentialLink.vue'

  const linksList = [
    {
      title: 'Instagram',
      caption: '@reigikai',
      icon: 'favorite',
      link: 'https://www.instagram.com/reigikai/'
    },
    {
      title: 'Facebook',
      caption: '@skc.skif.lv',
      icon: 'camera',
      link: 'https://www.facebook.com/groups/skc.skif.lv'
    },
    {
      title: 'TikTok',
      caption: '@reigikai',
      icon: 'slideshow',
      link: 'https://www.tiktok.com/@reigikai'
    },
    {
      title: 'Google Maps',
      caption: 'Our location on Google Maps',
      icon: 'public',
      link: 'https://goo.gl/maps/Jurn65vKomTaMhjcA'
    },
    {
      title: 'Apple Maps',
      caption: 'If you prefer to use Apple Maps',
      icon: 'apple',
      link: 'https://maps.apple.com/?address=614%20E%20Sahara%20Ave,%20Unit%2013,%20Las%20Vegas,%20NV%20%2089104,%20United%20States&ll=36.144998,-115.145824&q=614%20E%20Sahara%20Ave,%20Unit%2013&_ext=EiYpEBX0GfwRQkAxeyJTULDJXMA5juoZdiITQkBBF9m5DfrIXMBQBA%3D%3D'
    }
  ]

  export default defineComponent({
    name: 'MainLayout',

    components: {
      EssentialLink
    },

    setup () {
      const leftDrawerOpen = ref(false)

      return {
        essentialLinks: linksList,
        leftDrawerOpen,
        toggleLeftDrawer () {
          leftDrawerOpen.value = !leftDrawerOpen.value
        }
      }
    }
  })
</script>
