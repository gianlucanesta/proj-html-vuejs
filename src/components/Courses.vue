<template>
    <div class="container">

        <section class="online-courses">
            <h3>join maxcoach at best</h3>
            <h4>
                latest online 
                <span>courses</span>
            </h4>
            <div class="course-selection">
                <div class="single-course" v-for="(course, index) in courses" :key="index">
                    <img
                           
                        :src="require(`../assets/img/${course.image}-480x298.jpg`)" 
                        alt="course">
                    <h5>
                        {{ course.dollars }}
                        <span>{{ course.pennies }}</span>
                    </h5>
                    <h6>{{ course.title }}</h6>
                    <div class="specifics">
                        <i class="far fa-file-alt"></i>
                        <span>{{ course.lessons }} Lessons</span>
                        <i class="far fa-user"></i>
                        <span>{{ course.students }} Students</span>
                    </div>
                </div>
            </div>

            <div class="circle">
                <i class="fas fa-circle"></i>
                <i class="fas fa-circle"></i>
                <i class="fas fa-circle"></i>
                <i class="fas fa-circle"></i>
                <i class="fas fa-circle"></i>

                <p>
                    Control your personal preference settings to get notified about <br> courses. 
                    <a href="#">
                        View all courses 
                        <i class="fas fa-long-arrow-alt-right"></i>
                    </a>
                </p>
            </div>
        </section>


    </div>    
</template>

<script>
export default {
  name: "Courses",
  data: function () {
      return {
          courses: [
            {
                image: 'course-02',
                dollars: '$40',
                pennies: '.00',
                title: 'Learning to Write as a Professional Author',
                lessons: '20',
                students: '50'
            },
            {
                image: 'stock-full-hd-03',
                dollars: '$0',
                pennies: '.00',
                title: 'Customer-centric Info-Tech Strategies',
                lessons: '24',
                students: '769'
            },
            {
                image: 'stock-full-hd-04',
                dollars: '$19',
                pennies: '.00',
                title: 'Open Programming Courses for Everyone: Python',
                lessons: '17',
                students: '62'
            }
        ]
      }
    }
};
</script>


<style lang="scss" scoped>
.container {
    width: 67%;

    h3 {
        padding-top: 25px;
        font-size: 15px;
        font-weight: 500;
        color: #797d80;
        letter-spacing: 2px;
        text-transform: uppercase;
    }
    h4 {
        margin-bottom: 60px;
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

    .online-courses {
        text-align: center;

        .course-selection {
            display: flex;
            justify-content: space-around;
            
            .single-course {
                flex-basis: calc(100% / 3 - 23px);
                border-radius: 6px; 
                box-shadow: 0px 8px 43px -17px rgba(0,0,0,0.25);
                // border: 1px solid white;

                &:hover {
                    box-shadow: 0px 8px 43px -17px rgba(0,0,0,0.45);
                }

                h5 {
                    color: #20ad96;
                    font-weight: 700;
                    font-size: 24px;
                    padding-top: 20px;

                    span {
                        font-size: 20px;
                        margin-left: -7px;
                    }
                } 
                
                h6 {
                    width: 95%;
                    font-size: 19px;
                    font-weight: 700;
                    line-height: 1.5;
                    padding-top: 10px;
                    padding-bottom: 30px;

                    &:hover {
                        color: #20ad96;
                        cursor: pointer;
                    }
                }
                
                h5 , h6  {
                    text-align: left;
                    padding-left: 20px;
                    padding-right: 30px;
                }

                img {
                    width: 370px;
                    border-radius: 6px 6px 0 0;
                }
            }
        }
    }
    .specifics {
        text-align: left;
        padding-left: 20px;
        padding-right: 30px;
        padding-bottom: 40px;

        i {
            font-size: 14px;
            padding-right: 3px;
            color: #8c89a2;
            cursor: pointer;
        }
        span {
            font-size: 15px;
            color: #8c89a2;
            padding-right: 30px;
            padding-left: 8px;
            cursor: pointer;
        }
    }
    .circle {
        margin-top: 30px;
        text-align: center;
    

        i {
            color: #d8d8d8;
            font-size: 8px;
            padding: 0 8px;
            cursor: pointer;
            

            &:first-child {
                font-size: 12px;
                color: black;
            }
        }

        p {
            color: #797d80;
            font-size: 17px;
            font-weight: 500;
            line-height: 1.7;
            padding-top: 50px;

            a {
                color: black;
                font-size: 18px;
                font-weight: 700;
                border-bottom: 1px solid #d8d8d8;
            } 
        }

        
    }

}














</style>