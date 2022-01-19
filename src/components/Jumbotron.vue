<template>
    <div class="jumbo-section d-flex justify-content-center align-items-center">
        <div class="d-flex justify-content-center row">
            <h1 class="d-flex justify-content-center">Commence Business</h1>
            <h2 class="d-flex justify-content-center">Distant Mentoring Program</h2>
            <a class="btn" href="#">
                Download free guidebook 
                <i class="ms-2 fas fa-long-arrow-alt-right"></i>
            </a>      
        </div>  
    </div>
</template>

<script>
export default {
  name: 'Jumbotron',
 
}
</script>


<style lang="scss" scoped>


.jumbo-section {
    background-color: beige;
    background-image: url(../assets/img/home-3-hero-bg.jpg);
    height: 676px;
    background-repeat: no-repeat;
    background-position-x: center;
    background-position-y: center;
    margin-top: 20px;
    
    h1,h2 {
        color: #ffffff;
    }

    h1 {
        font-size: 32px;
        font-weight: 700;
    }

    h2 {
        font-size: 64px;
        font-weight: 400;
        margin-bottom: 40px;
    }

    .btn {
        display: block;
        padding: 15px 20px;
        background-color: #ffffff;
        color: #1fad95;
        text-decoration: none;
        border-radius: 5px;
        font-weight: 700;
        width: 20%;
        font-size: 14px;
    }

    .btn:hover {
        background-color: #20ad96;
        border-color: 1px solid #20ad96;
        color: #fff;
        transition: background 1s, color 1s;
    }
}

</style> 