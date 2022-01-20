<template>
    <main>
        <Jumbotron />
        <Work />
        <Skill />
        <Courses />
        <Testimonials />
        <Transform />
        <Blogs />
        <Newsletter />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Work from "./Work.vue";
import Skill from "./Skill.vue";
import Courses from "./Courses.vue";
import Testimonials from "./Testimonials.vue";
import Transform from "./Transform.vue";
import Blogs from "./Blogs.vue";
import Newsletter from "./Newsletter.vue";

export default {
  name: 'Main',
  components: {
    Jumbotron,
    Work,
    Skill,
    Courses,
    Testimonials,
    Transform,
    Blogs,
    Newsletter
  },
 
};
</script>


<style lang="scss" scoped>

main {
  margin-top: 80px;
  // background-color: #f1f1f1;
}


</style> 