<template>
 
  <div class="container">
    <section class="trasform mt-100">
      <div class="image w-50 mr-50">
        <img src="../assets/img/home-3-team-image.png" alt="home-3-team-image">
        <img src="../assets/img/maxcoach-shape-05.png" alt="maxcoach-shape-05">
        <img src="../assets/img/maxcoach-shape-07.png" alt="maxcoach-shape-07">
        <img src="../assets/img/maxcoach-shape-01.png" alt="maxcoach-shape-01">
      </div>
      <div class="description w-50 mt-50">
        <h3>
            everything in 
            <span>maxcoach</span>
        </h3>
        <h4>
            we're here to 
            <span>trasform</span> 
            you
        </h4>
        <p>As learners, people can enjoy great companionship from MaxCoach mentors and educators. We can help you develop and grow at your best.</p>
        <a class="btn btn-reverse" href="#">Get Free Guide</a>
      </div>
    </section> 
  </div>
    
</template>

<script>
export default {
  name: 'Transform',
  
};
</script>


<style lang="scss" scoped>

.container {
    margin-top: 200px;
    margin-bottom: 50px;

}

.trasform {
    display: flex;

    .image {
        position: relative;

        img{
            

            &:first-child {
                position: relative;
                width: 90%;
                z-index: 1;
            }

            &:nth-child(2) {
                position: absolute;
                top: 100px;
                left: -100px;
            }

            &:nth-child(3) {
                position: absolute;
                bottom: -100px;
                left: 270px;
                width: 170px;
            }

            &:last-child {
                position: absolute;
                top: 340px;
                left: -250px;
            }
        }
    }

    .description {

        h3 {

            span {
                color: #000;
                font-weight: 500; 
            }
        }

        h4 {

            span {
                font-size: 40px;
                color: #20ad96;
                font-weight: 400;
            }
        }
        p {
            color: #797d80;
            line-height: 1.7;
            padding: 10px 0;
        }

        a { 
            padding: 14px 50px;
            font-weight: 700;
            background-color: #20ad96;
            color: white;
            transition: background 1s, color 1s;

            &:hover {
                background-color: #fff;
                color: #20ad96;
                border: 1px solid #20ad96;
            }
        }
    }
}

</style>