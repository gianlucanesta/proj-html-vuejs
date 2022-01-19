<template>
    <header>
      <!-- Header Section Start -->
      <div class="">
        <div class="top-bar row d-flex align-items-center justify-content-between">
          
          <!-- Header Main Menu Start -->
          <div class="main-menu col-5 ">
              
            <ul class="d-flex justify-content-end m-auto me-5 p-0 ">
              
              <li v-for="(link, index) in links" :key="index">
                <a :href="link.url">
                  <span class="menu-text">{{link.text}}</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>

              <!-- <li>
                <a href="#">
                  <span class="menu-text">Home</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>
              
              <li>
                <a href="#">
                  <span class="menu-text">Pages</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>

              <li>
                <a href="#">
                  <span class="menu-text">Courses</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>

              <li>
                <a href="#">
                  <span class="menu-text">Features</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>

              <li>
                <a href="#">
                  <span class="menu-text">Blog</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li>

              <li>
                <a href="#">
                  <span class="menu-text">Shop</span>
                  <span class="menu-toggle">
                    <i class="fas fa-chevron-down"></i>
                  </span>
                </a>
              </li> -->

            </ul>
            
          </div>
          <!-- Header Main Menu End -->


          <!-- Header Logo Start -->
          <div class="header-logo col-3 d-flex justify-content-start">
            <a href="#">
              <img class="dark-logo" src="../assets/dark-logo.png" alt="Dark Logo">
            </a>
          </div>
          <!-- Header Logo End -->


          <!-- Header Right Menu Start -->
          <div class="right-menu col-4">
            <div class="d-flex justify-content-center m-auto p-0">
              
              <div class="d-flex align-items-center lex-column">
               <!-- Header Cart Start -->
                <div class="header-cart me-4">
                  <a class="header-cart-btn" href="#">
                    <span class="cart-items">0</span>
                    <i class="fas fa-shopping-cart"></i>
                  </a>
                </div>
                <!-- Header Cart End -->
              </div>

              <div class="d-flex align-items-center">
                <!-- Header User Start -->
                <div class="header-user me-4">
                    <a href="#"><i class="far fa-user-circle"></i></a>
                </div>
                <!-- Header User End -->
              </div>

              <div class="d-flex align-items-center">
                <!-- Header Search Start -->
                <div class="search-bar-container">
                    <div class="search-bar me-5">

                      <svg xmlns="http://www.w3.org/2000/svg" style="display:none">
                        <symbol xmlns="http://www.w3.org/2000/svg" id="sbx-icon-search-9" viewBox="0 0 40 41">
                              <path d="M25.25 32.2c-2.417 1.307-5.184 2.05-8.126 2.05C7.667 34.25 0 26.58 0 17.123 0 7.667 7.667 0 17.124 0 26.582 0 34.25 7.667 34.25 17.124c0 3.277-.92 6.338-2.517 8.94.29.18.563.397.814.65l6.105 6.103c1.8 1.8 1.795 4.722 0 6.52-1.8 1.8-4.72 1.798-6.52 0l-6.104-6.105c-.314-.313-.572-.66-.777-1.03zm-8.126-4.116c6.053 0 10.96-4.907 10.96-10.96 0-6.052-4.907-10.96-10.96-10.96-6.052 0-10.96 4.908-10.96 10.96 0 6.053 4.908 10.96 10.96 10.96z"
                          fill-rule="evenodd" />
                        </symbol>
                        <symbol xmlns="http://www.w3.org/2000/svg" id="sbx-icon-clear-5" viewBox="0 0 20 20">
                          <path d="M10 20c5.523 0 10-4.477 10-10S15.523 0 10 0 0 4.477 0 10s4.477 10 10 10zm1.35-10.123l3.567 3.568-1.225 1.226-3.57-3.568-3.567 3.57-1.226-1.227 3.568-3.568-3.57-3.57 1.227-1.224 3.568 3.568 3.57-3.567 1.224 1.225-3.568 3.57zM10 18.272c4.568 0 8.272-3.704 8.272-8.272S14.568 1.728 10 1.728 1.728 5.432 1.728 10 5.432 18.272 10 18.272z"
                          fill-rule="evenodd" />
                        </symbol>
                      </svg>

                      <form novalidate="novalidate" onsubmit="return false;" class="searchbox sbx-custom">
                        <div role="search" class="sbx-custom__wrapper">
                          <input type="search" name="search" placeholder="Search..." autocomplete="off" required="required" class="sbx-custom__input">
                          <button type="submit" title="Submit your search query." class="sbx-custom__submit">
                            <svg role="img" aria-label="Search">
                              <use xlink:href="#sbx-icon-search-9"></use>
                            </svg>
                          </button>
                          <button type="reset" title="Clear the search query." class="sbx-custom__reset">
                            <svg role="img" aria-label="Reset">
                              <use xlink:href="#sbx-icon-clear-5"></use>
                            </svg>
                          </button>
                        </div>
                      </form>

                    </div>
                </div>

              </div>
              <!-- Header Search End -->
            </div>
          </div>
          <!-- Header Right Menu End -->

        </div>
      </div>
      <!-- Header Section End -->

    </header>
</template>

<script>
export default {
  name: 'Header',
  data: function() {
    return {
      links: [
        {
          text: 'Home',
          url: '#'
        },
        {
          text: 'Pages',
          url: '#'
        },
        {
          text: 'Courses',
          url: '#'
        },
        {
          text: 'Features',
          url: '#'
        },
        {
          text: 'Blog',
          url: '#'
        },
        {
          text: 'Shop',
          url: '#'
        },
      ]
      
    }
  }
}
</script>


<style lang="scss" scoped>
@import '../style/variables';

.top-bar {
  height: 80px;
}

a:hover {
  color: #1FAD95;
}


// Main Menu
.main-menu {
  
  li  {
    margin: 0px 15px;
  }

}

.fa-chevron-down {
    margin-left: 10px;
    font-size: 8px;
  }

// Logo
.header-logo {
  
  .dark-logo {
    margin-left: 20px;
  }
  
}

.dark-logo {
  width: 155px;
}

// Right Menu
.right-menu {
  text-align: right;
}

.header-cart {
  font-size: 17px;
  position: relative;
  padding: 7px 9px 7px 0;
 
  
}

.cart-items {
  text-align: center;
  vertical-align: middle; 
  width: 15px;
  height: 15px;
  font-size: 9px;
  color: white;
  background-color: #1FAD95;
  border: 1px solid #1FAD95;
  border-radius: 50px;
  position: absolute;
  top: 0;
  right: 0;
}

.header-user {
  font-size: 17px;
}


/* Search Bar */
.sbx-custom {
  display: inline-block;
  position: relative;
  width: 230px;
  height: 48px;
  white-space: nowrap;
  box-sizing: border-box;
  font-size: 16px;
}

.sbx-custom__wrapper {
  width: 100%;
  height: 100%;
}

.sbx-custom__input {
  display: inline-block;
  transition: box-shadow .4s ease, background .4s ease;
  border: 0;
  border-radius: 6px;
  box-shadow: inset 0 0 0 1px #FFFFFF;
  background: #F5F5F5;
  padding: 0;
  padding-right: 76px;
  padding-left: 12px;
  width: 100%;
  height: 100%;
  vertical-align: middle;
  white-space: normal;
  font-size: inherit;
  appearance: none;
}

.sbx-custom__input::-webkit-search-decoration, .sbx-custom__input::-webkit-search-cancel-button, .sbx-custom__input::-webkit-search-results-button, .sbx-custom__input::-webkit-search-results-decoration {
  display: none;
}

.sbx-custom__input:hover {
  box-shadow: inset 0 0 0 1px #e6e6e6;
}

.sbx-custom__input:focus, .sbx-custom__input:active {
  outline: 0;
  box-shadow: inset 0 0 0 1px #1FAD95;
  background: #FFFFFF;
}

.sbx-custom__input::placeholder {
  color: #BBBBBB;
}

.sbx-custom__submit {
  position: absolute;
  top: 0;
  right: 0;
  left: inherit;
  margin: 0;
  border: 0;
  border-radius: 0 5px 5px 0;
  background-color: rgba(255, 255, 255, 0);
  padding: 0;
  width: 49px;
  height: 100%;
  vertical-align: middle;
  text-align: center;
  font-size: inherit;
  user-select: none;
}

.sbx-custom__submit::before {
  display: inline-block;
  margin-right: -4px;
  height: 100%;
  vertical-align: middle;
  content: '';
}

.sbx-custom__submit:hover, .sbx-custom__submit:active {
  cursor: pointer;
}

.sbx-custom__submit:focus {
  outline: 0;
}

.sbx-custom__submit svg {
  width: 15px;
  height: 15px;
  vertical-align: middle;
  fill: #1FAD95;
}

.sbx-custom__reset {
  display: none;
  position: absolute;
  top: 11px;
  right: 49px;
  margin: 0;
  border: 0;
  background: none;
  cursor: pointer;
  padding: 0;
  font-size: inherit;
  user-select: none;
  fill: rgba(0, 0, 0, 0.5);
}

.sbx-custom__reset:focus {
  outline: 0;
}

.sbx-custom__reset svg {
  display: block;
  margin: 4px;
  width: 19px;
  height: 19px;
}

.sbx-custom__input:valid ~ .sbx-custom__reset {
  display: block;
  animation-name: sbx-reset-in;
  animation-duration: .15s;
}

@keyframes sbx-reset-in {
  0% {
    transform: translate3d(-20%, 0, 0);
    opacity: 0;
  }
  100% {
    transform: none;
    opacity: 1;
  }
}








// .search-bar-container {
//     display: flex;
//     justify-content: center;
//     align-items: center;

//     /* TEST */
//     // background-color: #f3eeea;
//     border-radius: 4px;
//     // border: 1px solid #1fad95;
// }

// .search-bar {
//     display: flex;
//     align-items: center;
//     width: 230px;
//     padding: 13px 10px;
//     border-radius: 5px;

//     /* Test */
//     background-color: whitesmoke;
// }




// .search-bar: {
//   background-color: white;
//   border: 1px solid #1fad95;
//   .search-input {
//     background-color: white;
//   }
// }

// .search-bar i {
//     margin-right: 10px;
//     color: #1fad95;
//     cursor: unset;
// }



// .search-input {
//     font-size: 15px;
//     flex-grow: 1;
//     border: 0;
//     outline: none;
//     background-color: whitesmoke;
// }


</style> 