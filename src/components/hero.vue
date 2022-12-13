<template>
    <div class="hero-sec">
        <div class="left">
            <h1>
                Multiplying your Wealth
            </h1>
            <p>Simple. Transparent. Unbiased</p>
            <a href="#" class="lnk-btn">
                Book A Call
            </a>
        </div>
        <div class="right">
            <img :src="rightimg" alt="finance-img">
        </div>
    </div>
    
</template>
<script>
export default {
  name: 'Hero',
  data(){
    return {
        rightimg: require("../assets/rimg.png")
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300&display=swap');
    img{
        max-width: 100%;
        object-fit: cover;
    }
    a{
        display: inline-block;
        text-decoration: none;
        font-family: 'Poppins', sans-serif;
    }
    h1,p{
        margin: 0;
        font-family: 'Poppins', sans-serif;
    }

    .hero-sec{
        display: flex;
        max-width: 90%;
        margin: 0 auto;
        gap: 2em;
        flex-wrap: wrap-reverse;
        align-items: center;    
        min-height: calc(100vh - 100px);
    }
    .hero-sec>*{
        flex: 1 1 25em;
    }
    .hero-sec h1{
        font-weight: 700;
        font-size: clamp(40px,5vw,70px);
        line-height: 1.2;
        background: rgb(241,241,241);
        background: linear-gradient(90deg, rgba(241,241,241,1) 0%, rgb(241, 161, 29) 100%, #F1A11D 100%);
        background-clip: text;
        -webkit-text-fill-color: transparent;
}
    .hero-sec p{
        font-weight: 500;
        font-size: 30px;
        color:rgb(241,204,143);
        padding: 1em 0;

    }
    .hero-sec a{
        font-weight: 700;
        font-size: 20px;
        padding: 0.3em 1em;
        background-color: #fafafa;
        /* #154954; */
        color: rgb(0, 0, 0);
        border-radius: 50px;
        -webkit-border-radius: 50px;
        -moz-border-radius: 50px;
        -ms-border-rodius: 50px;
        -o-border-radius: 50px;
        transition: 0.3s ease-in-out;
        -webkit-transition: 0.35 ease-in-out;
        -moz-transition: 0.3s ease-in-out;
        -ms-transition: 0.35 ease-in-out;
        -o-transition: 0.3s ease-in-out;

    }
    .hero-sec a:hover{
        background-color:  rgba(42, 42, 42, 0.939);
        color: #fff;

    }
    
</style>