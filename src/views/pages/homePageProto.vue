<template>
    <section id="home">
        <nav>
            <h4 class="logo">VIO<br>LET</h4>
            <div class="ham">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </nav>
        
        <div class="col">
            <div class="pages">
                <span class="line"></span>
                <div id="sc">
                        <p>1</p>
                </div>
                <span class="line2"></span>
            </div>


            <div class="landing">
                <div class="titik">
                    <img class="satu" src="../../assets/Frame 31.png" width="35">
                    <img class="dua" src="../../assets/Frame 31.png" width="35">
                    <img class="tiga" src="../../assets/Frame 31.png" width="35">
                </div>
                <div class="in">
                    <h4>Introduction</h4>
                    <h1>travel BNJ.</h1>
                    <p>Hi, im Muhammad Rizki. A Front End Devoloper based in Indonesia<br>Focused on Creating web design and web devoloping.</p>
                </div>                
            </div>

        </div>
            <div class="hidden">
                <div class="media-main">
                    <a href="#">instagram</a>
                    <a href="#">twitter</a>
                    <a href="#">whatsapp</a>
                </div>
            </div>
            <div class="hidden">
                <div class="copyright">
                    <p>2023 - Muhammad Rizki</p>
                </div>
            </div>
            <a class="arrow-down" href="#about">
                <img src="../../assets/icons8-down-arrow-24.png" alt="Down">
            </a>
    </section>
  </template>
    
  <script>
  
  export default {
      components: {
      },
      mounted() {
      
    }
  }
  
  </script>
  
  <style scoped>
  
  @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Barlow+Condensed:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Poppins:wght@100;200;300;500;600;700&display=swap');
  
  /* ===============================================Home===================================================== */
  
#home {
    width: 100vw;
    height: 100vh;
    position: relative;
    box-sizing: border-box;
    display: grid;
    align-content: center;
    overflow-x: hidden;
    background-image: linear-gradient(to right, #10131D,#151927,#1F2334,#4a3a4f);
    z-index: -1;
}

#home nav {
    box-sizing: border-box;
    display: flex;
    align-items: center;
    justify-content: space-between; 
    padding: 20px 50px;
    width: 100%;
    position: fixed;
}


#home nav h4.logo {
    letter-spacing: 5px;
    font-size: .8rem;
    cursor: pointer;
    color: #FFFFFF;
}

#home nav .ham {
    display: grid;
    position: relative;
    align-items: center;
    justify-content: center;
    width: 35px;
    height: 35px;
    box-sizing: border-box;
    padding: 8px 10px;
    border-radius: 50%;
    background-color: #ffffff40;
    cursor: pointer;
}
#home nav .ham span {
    width: 10px;
    height: 1px;
    background-color: #fff;
}



/* Landing */

#home .col {
    display: flex;
    gap: calc(5vw + 1em);
    position: fixed;
    align-self: center;
}

#home .landing {
    display: grid;
    align-self: center;
    gap: 5px;
    padding-right: 5px;
    position: relative;
}
#home .landing h4 {
    font-size: .6rem;
    letter-spacing: 1px;
    font-weight: 500;
    transition: all .5s ease-out;
    color: #FFFFFF;
}
#home .landing h1 {
    font-size: calc(1vw + 3rem);
    font-weight: 500;
    margin-bottom: 10px;
    transition: all .7s ease-out .1s;
    color: #FFFFFF;
}
#home .landing p {
    font-size: .6rem;
    font-weight: 300;
    letter-spacing: 2px;
    color: #bcbcbc;
    line-height: 2;
    transition: all .6s ease-out .3s;
}
#home .landing .in {
    overflow-x: hidden;
}

#home .landing .titik {
    position: absolute;
    display: flex;
    gap: 7px;
    top: -29px;
    z-index: -2;
    overflow-x: hidden;
}

#home .landing .titik img.satu {
    opacity: .4;
    position: relative;
    left: -120px;
    transition: all .5s ease-out;
    animation: titik .5s .4s ease-in-out forwards;
}
#home .landing .titik img.dua {
    opacity: .6;
    position: relative;
    left: -120px;
    transition: all .5s ease-out;
    animation: titik .5s .3s ease-in-out forwards;
}
#home .landing .titik img.tiga {
    opacity: .8;
    position: relative;
    left: -120px;
    transition: all .5s ease-out;
    animation: titik .5s .2s ease-in-out forwards;
}

@keyframes titik {
    0% {
        left: -120px;
    }
    100% {
        left: 0;
    }
}


#home .pages {
    height: 50vh;
    width: max-content;
    display: grid;
    justify-items: center;
    align-self: center;
    margin-left: calc(1vw + 2rem);
    overflow: visible;
    position: relative;
}
#home .pages span:nth-child(1) {
    position: absolute;
    display: grid;
    top: 265px;
    width: 1px;
    height: 130px;
    background-color: #ffffff7f;
    /* animation: pages-range .5s .5s ease-out forwards; */
    transition: all .4s ease-out;
}

#home .pages span:nth-child(3){
    position: absolute;
    display: grid;
    bottom: 265px;
    width: 1px;
    height: 130px;
    background-color: #ffffff7f;
    /* animation: pages-range .5s .5s ease-out forwards; */
    transition: all .4s ease-out;
}

/* .line.default {
    height: 0;
} */


@keyframes pages-range {
    0% {
        height: 0;
    }
    100% {
        height: 130px;
    }
}


#home .pages div:nth-child(2) {
    width: 40px;
    height: 40px;
    display: flex;
    position: absolute;
    justify-content: center;
    align-self: center;
    border: 1px solid #fff;
    border-radius: 50%;
    overflow: hidden;
}
#home .pages a {
    font-size: .85rem;
}
/* #home .pages a:nth-child(2) {
    display: grid;
    transform: translateY(39px);
    gap: 5px;
    transition: all .5s ease-out;
    position: relative;
} */
#home .pages #sc p:nth-child(1) {
    position: absolute;
    top: 9px;
    transition: all .4s ease-out;
}
#home .pages #sc p:nth-child(2) {
    position: absolute;
    bottom: -25px; 
    display: flex;
    transition: all .4s ease-out;
}
#home .pages #sc p:nth-child(3) {
    position: absolute;
    transition: all .4s ease-out;
    bottom: -25px; 
}
#home .pages #sc p:nth-child(4) {
    position: absolute;
    transition: all .4s ease-out;
    bottom: -25px; 
}


#home .num-pages {
    height: 200px;
    width: max-content;
    position: fixed;
    display: flex;
    justify-self: flex-end;
    justify-items: center;
    align-items: center;
    align-self: center;
    right: calc(1vw + 3rem);
    gap: 40px;
}
#home .num-pages .number {
    display: grid;
}
#home .num-pages .number a {
    font-size: .75rem;
    display: flex;
    justify-content: center;
    font-weight: 300;
}
#home .num-pages .range {
    width: 1.5px;
    height: 120%;
    background-color: #ffffff54;
    position: relative;
}
#home .num-pages .range span {
    width: 2px;
    height: 50px;
    position: absolute;
    top: 0;
    background-color: #fff;
}


/* media */

#home .media-main {
    width: fit-content;
    position: fixed;
    display: flex;
    align-self: self-end;
    gap: 20px;
    left: calc(1vw + 2rem);
    bottom: calc(1vw + 1rem);
}
#home .media-main a {
    text-decoration: none;
    letter-spacing: 1px;
    font-weight: 300;
    font-size: .75rem;
    color: #ffffffa2;
}

#home .copyright {
    width: 100%;
    position: fixed;
    display: none;
    align-self: flex-end;
    gap: 20px;
    left: calc(1vw + 2rem);
    bottom: calc(1vw + 1rem);
    justify-content: space-between;
}
#home .copyright p {
    letter-spacing: 1px;
    font-weight: 300;
    font-size: .6rem;
    color: #ffffffa2;
}


#home .arrow-down {
    /* background-color: #ffffff0b; */
    width: 40px;
    height: 40px;
    box-sizing: border-box;
    position: fixed;
    display: flex;
    justify-content: center;
    align-items: center;
    justify-self: end;
    align-self: flex-end;
    right: calc(1vw + 2rem);
    bottom: calc(1vw + 1rem);
    border-radius: 50%;
    cursor: pointer;
    transition: all .4s ease-out;
    background-image: linear-gradient(to right, #ffffff21, #ffffff21);
    background-size: contain;
    background-repeat: no-repeat;
    background-position-y: -40px;
}
#home .arrow-down img {
    width: 20px;
    opacity: .5;
    transition: all .4s ease-out;
}
#home .arrow-down:hover, #home .arrow-down:hover img {
    background-position-y: 0px;
    opacity: 1;
}
  
  </style>  