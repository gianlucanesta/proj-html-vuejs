<template>
    <main>
        <Jumbotron />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";


export default {
  name: 'Main',
  components: {
    Jumbotron,
  },
 
};
</script>


<style lang="scss" scoped>

main {
  margin-top: 80px;
  
}


</style> 