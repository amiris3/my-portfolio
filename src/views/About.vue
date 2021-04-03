<template>
  <div class="about">
    <h2><router-link to="/"> &larr; {{  $t('navigation.about') }}</router-link></h2>
    <p>{{  $t('about.presentation') }}</p>
    <p>{{  $t('about.hobbies') }}</p>

    <div class="col col1">
      <h4>{{  $t('about.i-speak') }}</h4>
      <ul>
        <li :key="language" v-for="language in  $t('about.foreign-lang')">{{ language }}</li>
      </ul>
    </div>

    <div class="col col2">
      <h4>{{  $t('about.i-code-in') }}</h4>
      <ul>
        <li>PHP, SQL</li>
        <li>C/C++</li>
        <li>Java</li>
        <li>Twig (Drupal, Symfony)</li>
        <li>Dart (Flutter)</li>
        <li>Haskell</li>
      </ul>
    </div>
  </div>
</template>
