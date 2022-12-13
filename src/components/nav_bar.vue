<template>
    <section class="header">
        <a href="#" class="logoo">
            <img :src="logo" alt="logo" class="logo">
        </a>
        <div class="toggleMenu" @click="toggleMenu()"></div>
        <nav class="navigation">
            <ul>
                <li>
                    Platform
                </li>
                <li>Features</li>
                <li>How it Works</li>
            </ul>
        </nav>
        <button class="btn">Get The App</button>
            <!-- <img :src="logo" alt="icon"> -->
        
    </section>

    
</template>

<script>

export default {
  name: 'Nav_bar',
  el: '.header',
  data(){
    return {
        logo: require("../assets/Loggo.png"),
    }
  },
  components: {
  },
//   methods: {
//     toggleMenu()
//     {
//         console.log("Toggling menu")
//      const toggleMenu=this.$el.queryselector (".toggleMenu");
//      const navigation=this.$el.querySelector(".navigation");
//      toggleMenu.classList.toggle("active");
//     }
    
//   }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300&display=swap');

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
.header {

    margin:0 3em;
    margin-top: 15px;
    padding: 10px;
    display:flex;
    max-width: 100vw;
    height: 50px;
    /* background-color: rgba(255, 255, 255, 0.15);  
 backdrop-filter: blur(5px); */
    justify-content: flex-end;
    align-items: center;
    
}
.logoo {
    margin-right: auto;
}
.header a img{
    
    padding: 20px;
    width: 180px;
    height: 70px;
    margin-right: 20px;
    flex-shrink: 0;


}
.header ul {
    display: flex;
    margin: 0px;
    padding: 0px;
    list-style: none;
    font-family: 'Poppins', sans-serif;
}
.header ul li {
    margin-right: 15px;
    margin-left: 15px;
    color: rgba(255, 183, 67, 0.776);
    font-size: 15px;
    font-weight: 500;
    font-family: 'Poppins', sans-serif;
}
.header ul li:hover{
    color: rgb(241,204,143);
    cursor: pointer;
}
.header ul li:after{
    display: block;
    content: "";
    width: 0;
    height: 3px;
    margin: 1px auto;
    background-color: rgb(241,204,143);
    border-radius: 5px;
    -webkit-bonder-radius: 5px;
    -moz-border-radius: 5px;
    -ms-border-radius: 5px;
    -o-border-radius: 5px;
    transition: 0.3s ease-in-out;
    -webkit-transition: 0.3s ease-in-out;
    -moz-transition: 0.3s ease-in-out;
    -ms-transition: 0.3s ease-in-out;
    -o-transition: 0.3s ease-in-out;

}
.header ul li:hover::after{
    width: 50px;
}
.btn{
    margin-left: 15px;
    width: 130px;
    height: 30px;
    /* padding: 9px 25px; */
    background-color: rgb(255, 255, 255);
    color: rgb(0, 0, 0);
    border-radius: 50px;
    border: none;
    cursor: pointer;
    font-weight: 700;
    font-family: 'Poppins', sans-serif;
}
.btn:hover{
    background-color: rgba(42, 42, 42, 0.939);
    transition: all 0.3s ease 0s;
    color: #fff;
    
    
}
@media screen and (max-width:740px){
    .navigation{
        display: none;
    }
    
}

/*@media screen and (max-width:900px){
    
    /* .toggleMenu {
        position: absolute;
        right: 5%;
        background-image: url(~@/assets/icon1.png);
        background-position: center;
        background-repeat: no-repeat;
        background-size:30px;
        width: 30px;
        height: 30px;
        padding: 2em;
        z-index: 1000;
        transition: background-size 0.3s ease-in-out;
        -webkit-transition: background-size 0.3s ease-in-out;
        -moz-transition: background-size 0.3s ease-in-out;
        -ms-transition: background-size 0.3s ease-in-out;
        -o-transition: background-size 0.3s ease-in-out;

    }
    .toggleMenu.active {
        position:fixed;
        background-image: url(~@/assets/close.svg);
        background-size: 25px;
    }
    .navigation{
        justify-content:center;
        align-items:center;
        flex-direction: column;
        max-height: 0;
        opacity: 0;
        transform-origin: top;
        transform: scale(1,0);
    }
    .navigation.active {
        position: fixed;
        inset: 0;
        margin: auto;
        max-height: 100%;
        opacity: 1;
        background-color: black;
        color: aliceblue;
    } */

</style>
