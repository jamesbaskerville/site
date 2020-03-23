<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn to="/" flat dense icon="chevron_right" />
        <q-toolbar-title>
              james baskerville
        </q-toolbar-title>

        <q-tabs align="center" dense breakpoint="0">
          <q-route-tab
            name="code"
            label="code"
            to="/code"
            exact
          />
          <q-route-tab
            name="music"
            label="music"
            to="/music"
            exact
          />
        </q-tabs>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',

  components: {},

  data() {
    return {
      links: [
        {
          title: 'Github',
          caption: 'github.com/jamesbaskerville',
          icon: 'code',
          link: 'https://github.com/jamesbaskerville',
        },
        {
          title: 'LibFasc Game',
          caption: 'jamesbaskerville.github.io/libfasc',
          icon: 'play_arrow',
          link: 'https://jamesbaskerville.github.io/libfasc',
        },
      ],
    };
  },
};
</script>
