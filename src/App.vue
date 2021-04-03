<template>
  <div id="app" class="wrapper">
      <main>
        <router-view/>
      </main>

      <div class="container">
        <input id="burger" type="checkbox"/>
        <label for="burger">
          <span></span>
          <span></span>
          <span></span>
        </label>
        <nav>
          <ul>
            <li class="nav-item">
              <div class="dropdown">
                <div class="red">
                  <button class="dropbtn">
                    &lsaquo; {{  $t('navigation.language') }} &rsaquo;
                  </button>
                </div>
                <LocaleSwitcher/>
              </div>
            </li>
            <li class="nav-item">
              <router-link to="/about-me">{{  $t('navigation.about') }}</router-link>
              <div class="list-item">
                <div class="small-item">
                  <div class="smaller-item"></div>
                </div>
              </div>
            </li>
            <li class="nav-item">
              <router-link to="/projects">{{ $t('navigation.projects') }}</router-link>
              <div class="list-item">
                <div class="small-item">
                  <div class="smaller-item"></div>
                </div>
              </div>
            </li>
            <li class="nav-item"><router-link to="/contact">{{ $t('navigation.contact') }}</router-link>
              <div class="list-item">
                <div class="small-item">
                  <div class="smaller-item"></div>
                </div>
              </div>
            </li>

          </ul>

        </nav><!-- end navigation -->
      </div>
    </div>
</template>

<style>
@import "assets/style.css";
</style>

<script>
import LocaleSwitcher from '@/components/LocaleSwitcher'
export default {
  components: { LocaleSwitcher }
}
</script>
