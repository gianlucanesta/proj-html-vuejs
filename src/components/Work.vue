<template>
    <div class="work-culture">
        <div class="container">
            
            <section class="work d-flex">
                <div class="description">
                    
                    <h3>everything in 
                        <span>maxcoach</span>
                    </h3>

                    <h4>Learn about our 
                        <span>Work Culture</span> 
                        at MaxCoach
                    </h4>

                    <p>Spend some time to visit our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.</p>

                    <p>Have questions? 
                        <a href="#">Get Free Guide 
                            <i class="fas fa-long-arrow-alt-right"></i>
                        </a>
                    </p>
                </div>
                <div class="content">
                    <img src="../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="stock">
                    <img src="../assets/img/maxcoach-shape-07.png" alt="maxcoach">
                    <img src="../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="about">
                    <img src="../assets/img/maxcoach-shape-02.png" alt="maxcoach">
                    <img src="../assets/img/maxcoach-shape-08.png" alt="maxcoach">
                </div>
            </section>
        </div>
        <div class="number-container d-flex justify-content-center">
            
            <section class="number d-flex justify-content-around">
                <div class="box">
                    <h5>129+</h5>
                    <span>enrolled learners</span>
                </div>
                <div class="box">
                    <h5>80</h5>
                    <span>finished sessions</span>
                </div>
                <div class="box">
                    <h5>4%</h5>
                    <span>satisfaction rate</span>
                </div>
            </section>
        </div>
        
        
    </div>
</template>

<script>
export default {
  name: 'Work',
  
};
</script>

<style lang="scss" scoped>


.work-culture{
    margin-top: 150px;

    .container {
        width: 65%;
    }
    .description {
        width: 60%;
        padding-right: 100px;

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
                color: #1fad95;
                font-weight: 700;
                border-bottom: 1px solid #d5dadd;
            }

        }
    }
    .content {
        position: relative;
        width: 80%;

        img:first-child {
            width: 570px;
            position: absolute;
            top: 10%;
            left: 18%;
            z-index: 1;
        }
        img:nth-child(2) {
            width: 150px;
            position: absolute;
            top: -5%;
            left: 83%;
        }
        img:nth-child(3) {
            width: 190px;
            position: absolute;
            top: -10%;
            left: 90%;
            border-radius: 5px;
            z-index: 2;
        }
        img:nth-child(4) {
            width: 130px;
            position: absolute;
            top: 85%;
            left: 77%;
            z-index: 2;
        }
        img:last-child {
            width: 165px;
            position: absolute;
            top: 63%;
            left: 20%;
        }
    }
    .number {
        margin: 100px 0;

        .box {
            margin: 0 65px;

            h5 {
                color: #20ad96;
                font-size: 50px;
                font-weight: 700;
                text-align: center;
            }
            span {
                display: block;
                color: #6c6c6b;
                font-weight: 700;
                font-size: 15px;
                text-transform: uppercase;
                margin-top: 10px;
                letter-spacing: 2px;
            }
        }
    }
}
</style>