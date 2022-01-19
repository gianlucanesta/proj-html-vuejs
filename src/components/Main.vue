<template>
    <main>
        <Jumbotron />
        <Work />
        
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Work from "./Work.vue";

export default {
  name: 'Main',
  components: {
    Jumbotron,
    Work,
  },
 
};
</script>


<style lang="scss" scoped>

main {
  margin-top: 80px;
  // background-color: #f1f1f1;
}


</style> 