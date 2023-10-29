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
      </div>
      <div class="header__item header__item2">
        <a href="#" class="header__item">Главная</a>
        <a href="#" class="header__item">Блог</a>
        <a href="#" class="header__item">Блог детэйлз</a>
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