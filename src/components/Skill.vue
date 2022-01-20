<template>
    <div class="container">
        <section class="d-flex">
        
            <div class="content">
                <img src="../assets/img/stock-full-hd-11-670x450.jpg" alt="stock"> 
                <img src="../assets/img/icon-youtube-play.png" alt="icon-youtube-play">
                <img src="../assets/img/maxcoach-shape-05.png" alt="maxcoach-shape-05">
                <!-- <img src="../assets/img/circle.JPG" alt="circle"> -->
                <img src="../assets/img/maxcoach-shape-07.png" alt="maxcoach-shape-07">
            </div>

            <div class="description">
                <h3>how we work</h3>

                <h4>
                    upgrade your skills 
                    <span> upgrade your life</span>
                </h4>

                <p>
                    Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped width new skills for new sets of insights into your careers.
                    MaxCoach accompany learners in every stage of learning. 
                </p>

                <p>
                    <a href="#">Download free guidebook 
                        <i class="fas fa-long-arrow-alt-right"></i>
                    </a>
                </p>
                
            </div>
        </section>
    </div>


    
</template>

<script>
export default {
  name: 'Skill',
  
};
</script>

///////////////////////////////////////////////////////

<style lang="scss" scoped>

.container {
    width: 65%;
    margin-bottom: 200px;

        .content {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            position: relative; 
            box-shadow: 0px 31px 42px -19px rgba(0,0,0,0.2);

            img:first-child {
                width: 100%;
                border-radius: 5px;
                position: absolute;
                top: 0;
                left: 0;
                z-index: 1;
            }
            img:nth-child(2) {
                width: 13%;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                cursor: pointer;
                z-index: 2;
            }
            img:nth-child(3) {
                position: absolute;
                top: 40px;
                left: -85px;
            }
            img:nth-child(4) {
                position: absolute;
                top: -30px;
                right: -110px;
                width: 50px;
            }
            img:last-child {
                width: 170px;
                position: absolute;
                top: 410px;
                right: -20px;
            }
        }

        .description {
            margin-top: 2%;
            width: 50%;
            margin-left: 80px;
            
        h3 {
            padding-top: 25px;
            font-size: 15px;
            font-weight: 500;
            color: #797d80;
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        h4 {
            padding-top: 10px;
            font-size: 48px;
            font-weight: 700;
            color: #3f3a64;
            text-transform: capitalize;

            span {
                color: #1fad95;
                font-weight: 400;
            }
        }
        p {
            margin-top: 25px;
            color: #797d80;
            font-size: 15px;
            line-height: 1.7;

            &:last-child {
                color:  #6c6c6b;
            }

            span {
                color: #6c6c6b;
                font-weight: 700;
            }
            a {
                color: #6c6c6b;
                font-weight: 700;
                border-bottom: 1px solid #d5dadd;
            }
        }
    }
}

</style>