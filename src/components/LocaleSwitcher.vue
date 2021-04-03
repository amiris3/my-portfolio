<template>
  <div class="dropdown-content">
    <a v-for="locale in locales" :key="locale.length" @click="switchLocale(locale.short)" href="#">{{ locale.long }}</a>
  </div>
</template>

<script>
import i18n from '@/i18n'
export default {
  name: 'LocaleSwitcher',
  methods: {
    switchLocale (locale) {
      if (i18n.locale !== locale) {
        i18n.locale = locale
      }
    }
  },
  data: function () {
    return {
      locales: [
        {
          long: 'Français',
          short: 'fr'
        },
        {
          long: 'English',
          short: 'en'
        }
      ]
    }
  }
}
</script>
