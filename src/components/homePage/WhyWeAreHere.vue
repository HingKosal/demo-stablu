<template>
    <div class="why_we_here">
        <h1>{{title}}</h1>
        <h3>{{more_detail}}</h3>
    </div>
</template>

<script>

export default {
  data() {
    return {
      title: 'Why we are Here?',
      more_detail: 'Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid. Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid'
    };
  }
}
</script>

<style>

  .body_container .body_content .body_wrapper .why_we_here {
    width: 100%;
    height: 300px;
    margin: 40px 0;
    text-align: center;
  }

  .body_container .body_content .body_wrapper .why_we_here h3 {
    padding: 0 180px;
    font-weight: normal;
  }
</style>