<template>
  <div class="container">
    <div class="row p-4">
      <div class="col-md-4 order-12">
        <div class="container">
          <TheTopRow />
        </div>
        <ul class="list-group pt-3 pb-3">
          <li class="list-group-item border border-warning">
            Blog Yazıları
            <span class="badge bg-primary text-dark hover">30</span>
          </li>

          <li class="list-group-item border border-warning">
            Faydalı Araçlar
            <span class="badge bg-danger text-dark hover">20</span>
          </li>
          <li class="list-group-item border border-warning">
            İnternet Siteleri
            <span class="badge bg-warning text-dark hover">15</span>
          </li>
        </ul>

        <div class="div" id="anotherbox">
          <ThePodList />
        </div>
      </div>

      <ThePosts />
    </div>
  </div>
</template>


<script>
import TheTopRow from "@/components/TheTopRow.vue";
import ThePosts from "@/components/ThePosts.vue";
import ThePodList from "@/components/ThePodList.vue";
export default {
  components: {
    ThePodList,
    TheTopRow,
    ThePosts,
  },
};
</script>


<style >

</style>