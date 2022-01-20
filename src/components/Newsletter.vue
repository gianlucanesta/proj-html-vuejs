<template>
 
  <div class="container">
    
    <section class="subscribe mt-100">
      <h4>
        Subscribe 
        <span>Newsletters</span>
      </h4>
      <p>
        Enter your email address to register to our newsletter subscription <br> 
        delivered on a regular basis!
      </p>
      <div class="newsletters mt-50">
          <input type="text" placeholder="Enter your email">
          <button>Subscribe</button>
      </div>
    </section> 
  </div>
</template>

<script>
export default {
  name: 'Newsletter',
  
};
</script>


<style lang="scss" scoped>

.container {
  width: 50%;
  margin-top: 50px;
  margin-bottom: 50px;

  .subscribe {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    p {
      font-size: 16px;
      color: #797d80;
      padding-top: 15px;
      line-height: 1.7;
      font-weight: 500;
      text-align: center;
    }

    h4 {

      span {
        color: #20ad96;
      }
    }

    .newsletters {
      width: 70%;

      input {
        padding: 12px 25px;
        width: 80%;
        border: none;
        color: #797d80;
        font-size: 16px;
        font-weight: 500;
      }

      button {
        padding: 12px 25px;
        border-top-right-radius: 5px;
        border-bottom-right-radius: 5px;
        border: none;
        background-color: #20ad96;
        border: 1px solid #20ad96;
        color: #fff;
        font-weight: 700;
        transition: background 2s, color 2s;
        cursor: pointer;

        &:hover {
          background-color: #fff;
          color: #20ad96;
          border: 1px solid #20ad96;
        }
      }
    }
  }
}















</style>