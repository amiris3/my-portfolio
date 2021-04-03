<template>
  <div class="projects">
    <h2><router-link to="/"> &larr; {{  $t('navigation.projects') }}</router-link></h2>
    <div class="col col1">
      <a class="project" href="#">
        <h4>{{  $t('projects[0].name') }}</h4>
        <img src="../assets/images/projects/EchecsEtMaths2020.png" alt=""/>
      </a>
    </div>
    <div class="col col2">
      <a class="project" href="https://github.com/amiris3/my_organizer">
        <h4>{{  $t('projects[1].name') }}</h4>
        <img src="../assets/images/projects/OrganiZer20201.png" alt=""/>
      </a>
    </div>
    <div class="col col1">
      <a class="project" href="https://github.com/amiris3/La-pousse-de-bambou">
        <h4>{{  $t('projects[2].name') }}</h4>
        <img src="../assets/images/projects/LaPousseDeBambou2020.png" alt=""/>
      </a>
    </div>
    <div class="col col2">
      <a class="project" href="#">
        <h4>{{  $t('projects[3].name') }}</h4>
        <img src="../assets/images/projects/ClubITLR2021.png" alt=""/>
      </a>
    </div>
  </div>
</template>
