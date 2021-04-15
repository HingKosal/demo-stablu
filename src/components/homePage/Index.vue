<template>
    <div class="body_container">
      <div class="body_content">
        <div class="body_wrapper">
            <Cover />
            <Project />
            <WhyWeAreHere />
        </div>
      </div>
    </div>
</template>

<script>
import Cover from './Cover.vue'
import Project from './Project.vue'
import WhyWeAreHere from './WhyWeAreHere.vue'

export default {
  components: {
    Cover,
    Project,
    WhyWeAreHere
  }
}
</script>

<style>

  .body_container {
    margin: 0;
  }

  .body_container .header_content {
    max-width: 1200px;
    margin: auto;
  }
  .body_container .body_content .body_wrapper {
    align-items: center;
    justify-content: space-between;
    max-width: 100%;
    margin: auto;
  } 

</style>

