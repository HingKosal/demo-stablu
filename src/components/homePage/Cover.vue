<template>
    <div class="cover">
        <div class="motto">
            <h1>{{motto}}</h1>
            <h3>{{more_detail}}</h3>
        </div>
        <div class="cover">
            <img :src="cover" alt="cover">
        </div>
    </div>
</template>

<script>
import cover from '../../assets/cover.png'

export default {
  data() {
    return {
      cover: cover,
      motto: 'Change your believe and Do the impossible',
      more_detail: 'Help Cambodia technology to the next level.'
    };
  }
}
</script>

<style>

  .body_container .body_content .body_wrapper .motto {
    width: 100%;
    margin-top: 50px !important;
    margin-bottom: 10px;
  }

  .body_container .body_content .body_wrapper .motto h1 {
    text-align: center;
    margin: 10px 0;
  }

  .body_container .body_content .body_wrapper .motto h3 {
    text-align: center;
    color: lightgray;
    margin: 0;
  }

  .body_container .body_content .body_wrapper .cover {
    width: 100%;
    margin: 20px 0;
    align-items: center;
  }

  .body_container .body_content .body_wrapper .cover img {
    display: block;
    margin: auto auto 50px auto;
    width: 70%;
  }
</style>
