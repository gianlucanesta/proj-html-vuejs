<template>
 
    <div class="container">
        
        <section class="testimonials">
            <div class="top-section">
                <h6>The MaxCoach team works really hard to hensure hight level of quality</h6>
                <p>I am happy with their arrangement of lessons and subjects. They</p>
            </div>
            <div class="description mr-50">
                <span>testimonials</span>
                <h4>
                    why do people 
                    <span>*hearts*</span> 
                    us?
                </h4>
                <p>Seeking for verbals of our service quality? Find them here. Everything is trasparent and straightforward for your sense of justification.</p>
                <a href="#">
                    View all 
                    <i class="fas fa-long-arrow-alt-right"></i>
                </a>
            </div>
            <div class="image">
                <h6>Professional team of specialists and passionate mentors at reach</h6>
                <p>I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                <img src="../assets/img/testimonial-avata-01.jpg" alt="testimonial-avata-01">
                <div class="contact">
                    <h6>madley pondor</h6> 
                    <span>/ IT Specialist</span>
                </div>
                <div class="bottom-section">
                    <img src="../assets/img/testimonial-avata-02.jpg" alt="testimonial-avata-02">
                    <div class="contact">
                        <h6>mina hollace</h6> 
                        <span>/ Freelancer</span>
                    </div>
                </div>
            </div>
        </section>
    </div>
    
</template>

<script>
export default {
  name: 'Testimonials',
  
};
</script>


<style lang="scss" scoped>

.container {
    width: 65%;
    margin-top: 250px;
}

.testimonials {
    position: relative;
    display: flex;
    
    .top-section {
        width: 50%;        
        position: absolute;
        top: -100px;
        right: 0;
        opacity: .2;

        h6 {
            font-size: 16px;
        }

        p {
            font-size: 14px;
            font-weight: 500;
        }
    }
    .description {
        width: 30%;
        margin-right: 150px;

        span {
            text-transform: uppercase;
            color: #797d80;
            font-size: 15px;
            font-weight: 500;
        }

        h4 {
            text-transform: capitalize;
            color: #000;
            font-size: 40px;
            font-weight: 700;

            span {
                color: #20ad96;
                font-size: 40px;
                font-weight: 400;
            }
        }
        
        p {
            color: #797d80;
            line-height: 1.7;
            padding: 10px 0;
        }

        a {
            
            color: #000;
            font-size: 18px;
            font-weight: 700;
            padding-top: 25px;
            border-bottom: 1px solid #e6e7e7;
        }
    }

    .image {
        width: 50%;
        

        img {
            width: 80px;
            border-radius: 50%;
            margin-top: 30px;
            vertical-align: middle;
            margin-right: 20px;
        }


        h6 {
            color: #000;
            font-size: 18px;
            font-weight: 700;
            padding-bottom: 10px;
        }

        p {
            font-size: 16px;
            color: #797d80;
            line-height: 1.7;
            font-weight: 500;
        }

        .contact {
            display: inline-flex;
            flex-direction: column;
            align-items: flex-start;

            h6 {
                text-transform: uppercase;
            }

            span {
                font-size: 14px;
                color: #797d80;
            }
        }

        .bottom-section {
            margin-top: 30px;
            opacity: .4;
            margin-left: 90px;
            
            box-shadow: inset 3px 37px 27px -11px rgba(148,148,148,0.5);
            img {
                width: 50px;
                border-radius: 50%;
                margin-top: 5px;
                vertical-align: middle;
                margin-left: 20px;
            }
            span {
                font-size: 12px;
                margin-top: -5px;
            }
        }
    }
}






</style>