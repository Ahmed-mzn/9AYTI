<template>
    <div>
        <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-inner">
            <div class="carousel-item active">
                <div>
                    <div class="sl  justify-center">
                      
                        <span class="v68_1">Bienvenue  sur Ghayti</span>
                        <span class="v68_2">Achetez librement En tout sécurité 
                            Avec un minimum d’effort</span>
                        <!-- <div class="hover:text-red-500 w-52 font-bold"> Bienvenue </div> -->
                        <router-link to="/magazin">
                        <button class="bg-blue-400 w-80 text-whitess font-bold p-4 rounded-xl ml-3/4 mt-96"> Magaziner </button>
                        
                    </router-link>
                     </div>
                </div>
            </div>
            </div>
            </div>

        <p class="v17 m-20">Nouvelle Arrivées</p>
        <!-- <div class="flex flex-col">
                <div class="v17-20 mx-40">
                <img src="sl1.jpg" class="cover" alt="" />
            </div>
            <p class="v68-4 mx-72 mt-4">Sac femme</p>
            <p class="text-blue-600 mx-72 mt-4 font"> 80000 MRU </p>
        </div> -->
        <div class="mx-5 mb-48  flex flex-col sm:flex-row justify-evenly">
            <div class="flex flex-col">
                    <img src="v1.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                       
                        <div>
                            <p class="text-center font-bold"> vetements </p>
                            <p class="text-center font-bold"> 87.00MRU </p>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                            <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                        </svg>
                        <!-- <div class="rounded-full bg-white shadow-xl"> -->
                            
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                        <!-- </div> -->
                        
                    </div>
            </div>
            <div class="flex flex-col">
                    <img src="so1.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                    <div>
                            <p class="text-center font-bold">crem nuit</p>
                            <p class="text-center font-bold"> 1500 MRU </p>
                    </div>
                    <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                     <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                     </svg>
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                    </div>  
            </div>
             <div class="flex flex-col">
                    <img src="p4.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                    <div>
                            <p class="text-center font-bold">parfum </p>
                            <p class="text-center font-bold"> 8000MRU </p>
                    </div>
                    <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                     <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                     </svg>
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                    </div>  
            </div>
        </div>
        <div class="mx-5 mb-48 flex flex-col sm:flex-row justify-evenly">
             <div class="flex flex-col">
                    <img src="p4.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                    <div>
                            <p class="text-center font-bold"> coo chanel </p>
                            <p class="text-center font-bold"> 6000 MRU </p>
                    </div>
                    <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                     <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                     </svg>
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                    </div>  
            </div>
             <div class="flex flex-col">
                    <img src="so3.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                    <div>
                            <p class="text-center font-bold">ecran </p>
                            <p class="text-center font-bold">600 MRU </p>
                    </div>
                    <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                     <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                     </svg>
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                    </div>  
            </div>
             <div class="flex flex-col">
                    <img src="p9.jpg" class="rounded-xl w-72 h-72" />
                    <div class="flex flex-row justify-evenly">
                    <div>
                            <p class="text-center font-bold"> Zara </p>
                            <p class="text-center font-bold"> 3500 MRU </p>
                    </div>
                    <svg xmlns="http://www.w3.org/2000/svg" className="h-5 w-5" viewBox="0 0 20 20" fill="currentColor" class="w-10 h-10 text-red">
                     <path fillRule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clipRule="evenodd" />
                     </svg>
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 2a4 4 0 00-4 4v1H5a1 1 0 00-.994.89l-1 9A1 1 0 004 18h12a1 1 0 00.994-1.11l-1-9A1 1 0 0015 7h-1V6a4 4 0 00-4-4zm2 5V6a2 2 0 10-4 0v1h4zm-6 3a1 1 0 112 0 1 1 0 01-2 0zm7-1a1 1 0 100 2 1 1 0 000-2z" clip-rule="evenodd" />
                        </svg>
                    </div>  
            </div>
        </div>
        <div class="v34-3 mt-72">
            <div class="mx-10 flex flex-row justify-between">
                <p class="v62-12 text-center w-1/3">
                    Des Cadeau et des Concours precieux pour nos clients fidèles
                </p>
                <p class="v62-12 text-center w-1/3 mt-40">
                    Des remises mansuelles considérables sur nos produits
                </p>
            </div>
        </div>
        <!-- <div class="v62_0">
            <div class="v37_7">
                <div class="v34_9"></div>
                <div class="v37_0"></div>
            </div>
            <div class="v37_6">
                <div class="v37_2"></div>
                <div class="v37_1"></div>
            </div>
            <div class="v37_8">
                <div class="v37_3"></div>
                <div class="v37_5"></div>
            </div>
        </div> -->
        <div class="flex flex-row mt-48 justify-center">
            <div class="bg-gray-300 shadow-xl rounded-full mr-5 w-32 h-32"><img src="paypal.png"  alt="" class="w-15 h-15 m-10"></div>
            <div class="bg-gray-300 shadow-xl rounded-full mr-5 w-32 h-32"><img src="logo.png"  alt="" class="w-16  h-16 m-8"></div>
            <div class="bg-gray-300 shadow-xl rounded-full w-32 h-32"><img src="cash.png"  alt="" class="w-16 h-16 m-9"></div>
        </div>
        
        <footer class="mt-48">
            <div
                class="bg-black text-white text-center font-mono font-bold h-12 mt-5"
            >
                © Copyright 2021. All Right Reserved for BOUTIQUE
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: "1"
};
</script>

<style lang="css" scoped>
/* * {
    box-sizing: border-box;
} */
/* body {
    font-size: 14px;
} */
.sl {
    background: url('sl1.jpg') ;
    background-size: cover;
    height: 88vh;
}
.v158_0 {
    width: 100%;
    height: 816px;
    background: url("sl1.jpg");
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
    opacity: 1;
    position: relative;
    top: 0px;
    left: 0px;
    overflow: hidden;
}
.v68_0 {
    width: 100%;
    height: 816px;
    background: url("../images/v68_0.png");
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
    opacity: 1;
    position: relative;
    top: 0px;
    left: 0px;
    overflow: hidden;
}
.v68_2 {
    width: 677px;
    color: rgba(12, 3, 68, 1);
    position: absolute;
    top: 405px;
    left: 1064px;
    font-family: Montserrat;
    font-weight: SemiBold;
    font-size: 37px;
    opacity: 1;
    text-align: center;
}
.v68_1 {
    width: 756px;
    color: rgba(22, 4, 94, 1);
    position: absolute;
    top: 290px;
    left: 1025px;
    font-family: Montserrat;
    font-weight: Bold;
    font-size: 55px;
    opacity: 1;
    text-align: left;
}
.v69_6 {
    width: 259px;
    height: 84px;
    background: rgba(55, 206, 211, 1);
    opacity: 1;
    position: absolute;
    top: 581px;
    left: 1280px;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    overflow: hidden;
}
.v69_13 {
    width: 190px;
    color: rgba(234, 234, 234, 1);
    position: absolute;
    top: 599px;
    left: 1329px;
    font-family: Poppins;
    font-weight: Bold;
    font-size: 30px;
    opacity: 1;
    text-align: left;
}
.v17 {
    color: #333;
    font-family: Montserrat;
    font-weight: Bold;
    font-size: 45px;
    opacity: 1;
}
.v17-20 {
    background: rgba(196, 196, 196, 1);
    width: 395px;
    height: 389px;
}
.v68-4 {
    color: #333;
    font-family: Poppins;
    font-weight: Medium;
    font-size: 27px;
    opacity: 1;
}
.v34-3 {
    background: url(discount.jpg);
    background-size: cover;
    width: 100%;
    height: 347px;
}
.v62-12 {
    color: #333;
    font-family: IM FELL English SC;
    font-weight: Regular;
    font-size: 44px;
    opacity: 1;
}
.v62-13 {
    color: #333;
    font-family: IM FELL English SC;
    font-weight: Regular;
    font-size: 44px;
    opacity: 1;
}
.v62_0 {
  width: 803px;
  height: 208px;
  background: url("../images/v62_0.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 0px;
  overflow: hidden;
}
.v37_7 {
  width: 208px;
  height: 208px;
  background: url("../images/v37_7.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 305px;
  overflow: hidden;
}
.v34_9 {
  width: 208px;
  height: 208px;
  background: rgba(239,234,234,1);
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 0px;
  border-radius: 50%;
  box-shadow: 4px 4px 19px rgba(0, 0, 0, 0.25);
}
.v37_0 {
  width: 179px;
  height: 110px;
  background: url("../images/v37_0.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 49px;
  left: 14px;
  overflow: hidden;
}
.v37_6 {
  width: 208px;
  height: 208px;
  background: url("../images/v37_6.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 595px;
  overflow: hidden;
}
.v37_2 {
  width: 208px;
  height: 208px;
  background: rgba(239,234,234,1);
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 0px;
  border-radius: 50%;
  box-shadow: 4px 4px 19px rgba(0, 0, 0, 0.25);
}
.v37_1 {
  width: 133px;
  height: 133px;
  background: url("../images/v37_1.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 37px;
  left: 37px;
  overflow: hidden;
}
.v37_8 {
  width: 208px;
  height: 208px;
  background: url("../images/v37_8.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 0px;
  overflow: hidden;
}
.v37_3 {
  width: 208px;
  height: 208px;
  background: rgba(239,234,234,1);
  opacity: 1;
  position: absolute;
  top: 0px;
  left: 0px;
  border-radius: 50%;
  box-shadow: 4px 4px 19px rgba(0, 0, 0, 0.25);
}
.v37_5 {
  width: 129px;
  height: 129px;
  background: url("../images/v37_5.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 41px;
  left: 42px;
  overflow: hidden;
}

.v68_1 {
  width: 756px;
  color: rgba(22,4,94,1);
  position: absolute;
  top: 469px;
  left: 1025px;
  font-family: Montserrat;
  font-weight: Bold;
  font-size: 55px;
  opacity: 1;
  text-align: left;
} 

.v68_2 {
  width: 677px;
  color: rgba(12,3,68,1);
  position: absolute;
  top: 584px;
  left: 1064px;
  font-family: Montserrat;
  font-weight: SemiBold;
  font-size: 37px;
  opacity: 1;
  text-align: center;
}

</style>
