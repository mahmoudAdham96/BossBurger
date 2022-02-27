<script setup>
import theHeader from "./components/nav/TheHeader.vue";
import Icon from "./components/menu/icon.vue";
import foot from  "./components/footer/footer.vue";
import prodCard from  "./components/cards/prodCard.vue";
components: {
  theHeader;
  Icon;
  foot;
  prodCard;
}
</script>

<template>
  <the-header> </the-header>
  <icon></icon>
  <prod-card> </prod-card>
  <foot> </foot>
</template>

<style>

#app {
  font-weight: normal;
}

</style>
