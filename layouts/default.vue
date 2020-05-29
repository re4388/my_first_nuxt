<template lang='pug'>
  v-app
    v-navigation-drawer(app v-model='drawer' )
      v-list
        v-list-item(v-for="(item, i) in items"
        :key="i" :to="item.to" router exact)
          v-list-item-action
            v-icon {{ item.icon }}
          v-list-item-content
            v-list-item-title(v-text="item.title")
    v-app-bar(app color='indigo')
      v-app-bar-nav-icon.white--text(@click.stop='drawer = !drawer')
      v-toolbar-title.white--text Github Fast Look
    v-content
      v-container
        nuxt
    v-footer(app color='indigo' )
      span.white--text &copy; 2020
</template>

<script>
export default {
  data () {
    return {
      drawer: true,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'about',
          to: '/about'
        },
        {
          icon: 'mdi-snowflake',
          title: 'myapp',
          to: '/myapp'
        }
      ],
      title: 'Vuetify.js'
    }
  }
}
</script>
