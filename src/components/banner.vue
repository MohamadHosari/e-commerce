<template>
    <div class="banner">
        <div class="container">
            <div class="banner-container">
                <div class="main-banner">
                    <div class="img-container">
                        <img class="img-ban" src="../assets/images/banner1.jpeg" alt="images" referrerpolicy="no-referrer"/>
                        <div class="img-content">
                            <span>
                                Banner
                            </span>
                            <h3>
                                Jeans
                            </h3>
                        </div>
                    </div>
                </div>
                <div class="category-banner">
                    <div class="top">
                        <div class="img-container">
                        <img class="img-ban" src="../assets/images/banner2.jpeg" alt="images" referrerpolicy="no-referrer"/>
                        <div class="img-content">
                            <span>
                                Banner
                            </span>
                            <h3>
                                Jeans
                            </h3>
                        </div>
                    </div>
                    <div class="img-container">
                        <img class="img-ban" src="../assets/images/banner3.png" alt="images" referrerpolicy="no-referrer"/>
                        <div class="img-content">
                            <span>
                                Banner
                            </span>
                            <h3>
                                Jeans
                            </h3>
                        </div>
                    </div>
                    </div>
                    <div class="bottom">
                        <div class="img-container">
                        <img class="img-ban" src="../assets/images/banner4.png" alt="images" referrerpolicy="no-referrer"/>
                        <div class="img-content">
                            <span>
                                Banner
                            </span>
                            <h3>
                                Jeans
                            </h3>
                        </div>
                    </div>
                    </div>
                </div>
                
            </div>
            <div class="banner-services">
                    <div v-for="n in 3" :key="n" class="sevice">
                    <span class="icon">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-truck-delivery" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"> <path stroke="none" d="M0 0h24v24H0z" fill="none"/> <circle cx="7" cy="17" r="2" /> <circle cx="17" cy="17" r="2" /> <path d="M5 17h-2v-4m-1 -8h11v12m-4 0h6m4 0h2v-6h-8m0 -5h5l3 5" /> <line x1="3" y1="9" x2="7" y2="9" /> </svg>
                    </span>
                    <div class="details">
                        <h6 class="head">FREE SHIPPING</h6>
                        <p class="para">On all orders above 100$</p>
                    </div>
                </div>
                </div>
        </div>

    </div>
</template>

<script setup>

</script>

<style >
    .banner{
        margin-top: 20px;
        padding: 40px 0px;
    }
    .banner .container{
        max-width: calc(1440px - 170px);
        width: 100%;
        margin: auto;
    }
    .banner-container{
        display: flex;
        justify-content: space-between;
        padding: 40px 0px;
    }
    .img-container{
        position: relative;
        height: 100%;
        width: 100%;
    }
    .img-container .img-content{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        background: #fff;
        border-radius: 4px;
        padding: 16px 32px;
        text-align: center;
    } 
    .img-content span{
        font-weight: 600;
        font-size: 12px;
        line-height: 13px;
        color: #121212;
        opacity: 0.4;
        text-transform: uppercase;
    }
    .img-content h3{
        font-weight: 600;
        font-size: 22px;
        line-height: 25px;
        color: #121212;
        text-transform: uppercase;
        margin-top: 5px;
    }
    .banner-content > div{
        flex: 0 0 calc(50% - 20px);
        max-width: calc(50% - 20px);
        width: 100%;
    }
    .img-container img{
        width: 100%;
        object-fit: cover;
    }
    .category-banner .top{
        display: flex;
        justify-content: space-between;
        margin-bottom: 30px;
    }
    .category-banner .top > div{
        flex: 0 0 calc(50% - 20px);
        max-width: calc(50% - 20px);
        width: 100%;
    }
    .banner-services{
        display: flex;
        justify-content: space-between;
        margin-bottom: 30px;
        align-items: center;
    }
    .banner-services > div{
        flex: 0 0 calc(33.33% - 20px);
        max-width: calc(33.33% - 20px);
        width: 100%;
        display: flex;
        align-items: center;
    }
    .sevice .details{
        margin-left: 13px;
    }
    .para, .head{
        margin-top: 0;
        margin-bottom: 0;
    }
    .details h6{
        font-weight: 600;
        font-size: 12px;
        line-height: 13px;
    }
    .details p{
        font-weight: 500;
        font-size: 12px;
        line-height: 22px;
        opacity: 0.9;
    }
    .banner{
        border-bottom: 1px solid #f8f8f8;
        margin-bottom: 100px !important;
    }
</style>