<template>
 
  <div class="container">
    <section class="blogs">
      <h3 class="text-center">read for more joyment</h3>
      <h4 class="text-center">
          latest from 
          <span>our blogs</span>
      </h4>
      <div class="blogger mt-50">
        <div class="blog">
          <img src="../assets/img/artist-blog-03-480x325.jpeg" alt="course">
          <h5>artist</h5>
          <h6>brush strokes energize trees in paintings</h6>
          <div class="blog">
            <i class="far fa-calendar"></i>
            <span>May 15, 2020</span>
            <i class="far fa-eye"></i>
            <span>688 views</span>
          </div>
        </div>
        <div class="blog">
          <img src="../assets/img/artist-blog-01-480x325.jpg" alt="stock-full-hd-03">
          <h5>artist</h5>
          <h6>pocket-sized notebooks hold miniature paintings</h6>
          <div class="info">
            <i class="far fa-calendar"></i>
            <span>May 15, 2020</span>
            <i class="far fa-eye"></i>
            <span>603 views</span>
          </div>
        </div>
        <div class="blog">
          <img src="../assets/img/artist-blog-02-480x325.jpg" alt="stock-full-hd-04">
          <h5>artist</h5>
          <h6>connection between self-portraits and identity</h6>
          <div class="info">
            <i class="far fa-calendar"></i>
            <span>May 15, 2020</span>
            <i class="far fa-eye"></i>
            <span>397 views</span>
          </div>
        </div>
      </div>
    </section> 
  </div>
    
</template>

<script>
export default {
  name: 'Blogs',
  
};
</script>


<style lang="scss" scoped>

.container {
  margin-bottom: 100px;
  margin-top: 200px;

  .blogs {
    
    h4 {


      span {
        color: #20ad96;
        font-weight: 400;
      }
    }

    .blogger {
      display: flex;
      justify-content: space-around;
      
      .blog {
        flex-basis: calc(100% / 3);
        margin: 0 10px;

        img {
          width: 100%;
        }

        h5 {
          color: #797d80;
          font-size: 14px;
          font-weight: 500;
          text-transform: uppercase;
          padding: 10px 0;
        }

        h6 {
          color: #333333;
          font-size: 20px;
          font-weight: 700;
          text-transform: capitalize;
          line-height: 1.7;
          padding-bottom: 20px;

          &:hover {
            color: #20ad96;
            cursor: pointer;
          }
        }

        span, i {
          color: #797d80;
          font-size: 15px;
        }

        span {
          padding-right: 30px;
        }
      }
    }
  }
}
</style>