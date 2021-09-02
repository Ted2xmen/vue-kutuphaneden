<template>
  <div class="home">
    <TheHero />
    <TheRowBanner />
     <div class="container">
      <hr class="bg-warning" />
      <TheRow />
      <hr class="bg-warning" />
    </div>
    <TheMain />

   

    <TheBoxes />
    <TheMailList />
  </div>
</template>

<script>
import TheRowBanner from "@/components/TheRowBanner.vue";
import TheMailList from "@/components/TheMailList.vue";
import TheBoxes from "@/components/TheBoxes.vue";
import TheRow from "@/components/TheRow.vue";
import TheHero from "@/components/TheHero.vue";
import TheMain from "@/components/TheMain.vue";

export default {
  name: "Home",
  components: {
    TheHero,
    TheMain,
    TheRow,
    TheBoxes,
    TheMailList,
    TheRowBanner,
  },
};
</script>



<style>
a {
  text-decoration: none !important;
}

li {
  list-style: none;
}

p {
  font-size: 16px;
}

body {
  overflow-x: hidden;
}
</style>