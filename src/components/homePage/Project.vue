<template>
    <div class="news">
        <div class="news_grid">
            <div class="child_news" v-for="pro in projects" :key="pro">
              <h2>{{pro.project_name}}</h2>
              <div class="child_news_body">
                <img :src="pro.project_image" alt="picture">
                <div class="text_news">
                  <h3>{{pro.title}}</h3>
                  <h4>{{pro.project_desc}}</h4>
                </div>
              </div>
            </div>
        </div>
    </div>
</template>

<script>
import project_image from '../../assets/cover.jpg'

export default {
  data() {
    return {
        projects: [
          {
            project_name: 'Project 1',
            project_image: project_image,
            title: 'title 1',
            project_desc: 'Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid container. Set the display....'
          },
          {
            project_name: 'Project 2',
            project_image: project_image,
            title: 'title 2',
            project_desc: 'Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid container. Set the display....'
          },
          {
            project_name: 'Project 3',
            project_image: project_image,
            title: 'title 3',
            project_desc: 'Set the display property to grid to make a block-level grid container. Set the display property to grid to make a block-level grid container. Set the display....'
          }
        ]
    };
  }
}
</script>

<style>

  .body_container .body_content .body_wrapper .news {
    margin: 10px 0;
    padding: 50px 0;
    width: 100%;
    background-color: #fff;
    color: black;
  }

  .body_container .body_content .body_wrapper .news .news_grid {
    padding: 0 30px;
    display: grid;
    grid-template-columns: auto auto auto;
  }
  
  .body_container .body_content .body_wrapper .news h2 {
    margin: 0 0 0 4px;
  }

  .body_container .body_content .body_wrapper .news .child_news {
      border-left: 2px solid grey;
  }

  .body_container .body_content .body_wrapper .news .child_news_body {
    display: flex;
  }

  .body_container .body_content .body_wrapper .news .child_news_body img {
    width: 40%;
  }

  .body_container .body_content .body_wrapper .news .child_news_body .text_news {
    margin: 0 10px;
    width: 100%;

  }

  .body_container .body_content .body_wrapper .news .child_news_body .text_news h3 {
    margin: 0;
  }

  .body_container .body_content .body_wrapper .news .child_news_body .text_news h4 {
    margin: 5px 0;
    color: #797777e7;
    font-weight: normal;
  }

</style>