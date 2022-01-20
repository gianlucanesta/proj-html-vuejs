<template>
    <div>
      <!-- Footer -->
      <footer class="footer">
          <div class="container">
              <div class="main-footer">
                  <div class="left-footer w-50">
                      <h5>Address</h5>
                      <span>
                          382 NE 191st #87394 Miami, FL 33179-3899 <br>
                          +1(305) 547-9909 (9am - 5pm EST, Monday - Friday) <br>
                          <a href="">support@maxcoach.com</a>
                      </span>
                      <div class="social">
                          <i class="fab fa-facebook-square"></i>
                          <i class="fab fa-twitter"></i>
                          <i class="fab fa-instagram"></i>
                          <i class="fab fa-linkedin"></i>
                      </div>
                  </div>
                  <div class="right-footer">
                      <div class="explore">
                          <h5>Explore</h5>
                          <div class="first-explore">
                              <ul v-for="(li, index) in footerExploreFirst" :key="index">
                                  <li>
                                    <a href="#">{{ li }}</a>
                                  </li>
                              </ul>

                          </div>
                          <div class="last-explore">
                              <ul v-for="(li, index) in footerExploreSecond" :key="index">
                                  <li>
                                      <a href="#">{{ li }}</a>
                                  </li>
                              </ul>
                          </div>
                      </div>

                      <div class="information">
                          <h5>Information</h5>
                          <ul v-for="(li, index) in information" :key="index">
                              <li>
                                  <a href="#">{{ li }}</a>
                              </li>
                          </ul>
                      </div>
                  </div>
                  
                </div>
              <span class="copyright m-auto">&copy; 2020 Maxcoach. All Rights Reserved</span>
          </div>

          <a class="arrow-up" href="#">
              <i class="fas fa-long-arrow-alt-up"></i>
          </a>
      </footer>
    </div>
</template>

<script>
export default {
  name: 'Footer',
  data: function () {
      return {
        footerExploreFirst: [
          'Start here',
          'Blog',
          'About us'
        ],
        footerExploreSecond: [
            'Success story',
            'Courses',
            'Contact us'
        ],
        information: [
            'Membership',
            'Purchase guide',
            'Privacy policy',
            'Teams of service'
        ]
      }
    }
 
}
</script>





<style lang="scss" scoped>


.footer {
    height: 400px;
    background-color: #171621;
    position: relative;

    .main-footer {
        display: flex;
        padding-top: 50px;
        
        .left-footer {
            span {
                color: #ababaa;
                font-size: 14px;
                line-height: 2.5;
                
                    a {
                        color: #ababaa;
                        text-decoration: none;
                    }
                }
                
            }
            h5 {
                color: #fff;
                font-size: 18px;
                font-weight: 700;
                padding-bottom: 15px;
            }

            .social {
                padding-top: 30px;

                i {
                    color: #ababaa;
                    font-size: 22px;
                    padding: 0 10px;
                    cursor: pointer;
                    transition: color, 1s;

                    &:hover {
                        color: #fff;
                    }
                }
            }
        }

        .right-footer {
            display: flex;

            .explore {
                display: flex;

                .first-explore {
                    position: relative;
                    top: 40px;
                    left: -60px;
                }

                .last-explore {
                    position: relative;
                    top: 40px;
                    left: 0;
                }
            }

            ul {

                li {

                    a {
                        color: #ababaa;
                        margin-left: -30px;
                        font-size: 15px;
                        text-decoration: none;
                        line-height: 2.5;

                        &:hover {
                            color: #fff;
                        }
                    }
                }
            }

            .information {
                margin-left: 50px;
            }

        }
    }

    span.copyright {
        color: #ababaa;
        display: block;
        text-align: center;
        position: relative;
        bottom: -40px;
    }

    a.arrow-up {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background-color: #20ad96;
        cursor: pointer;
        position: absolute;
        top: 80%;
        left: 94%;
    }

    a.arrow-up i {
        font-size: 30px;
        color: #fff;
    }


</style> 
