<script>

export default {




}
</script>
<template>
    
    <div>
    <header class="header">
      <div class="header__item header__item1">
        <img src="../assets/img/Logo.svg" alt="" />
        <h1>Interno</h1>
        
        <router-link to='/home'>Home</router-link>
        <router-link to='/projects'>Projects</router-link>
        <router-link to='/blog'>Blog</router-link>
        <router-link to='/blog_details'>Blog details</router-link>
        <router-link to='/project_details'>Project details</router-link>


      </div>
      <div class="header__item header__item2">

      </div>
    </header>
    </div>
</template>

<style lang="scss">
    .header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  &__item {
    display: flex;
    align-items: center;
  }
  &__item1 {
    gap: 3px;
    padding-left: 300px;
  }
  &__item2 {
    gap: 30px;
    padding-right: 300px;
  }
}
</style>