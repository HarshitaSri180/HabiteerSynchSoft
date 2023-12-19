<template>
    <!-- nine  -->
    <div class="container bg-purple p-5 rounded-5 ">
        <div class="my-2 row d-flex justify-content-between h-50">
            <!-- Left Column -->
            <div class="col-lg-6 col-md-12 top mb-4 mb-md-0 overflow-hidden">
                <div class="headings">
                    <div class="py-3 fw-bold h1" id="heading1">
                        Work with Us    
                    </div>
                </div>
                <div class="card rounded-4 p-2 workwithus-main-resp" style="width: 80%; height: 30rem;">
                    <div class="card border-0 py-2" :style="{ width: '', backgroundColor: '' }">
                        <div class="card-body">
                            <h1 class="card-title ">😎</h1>
                            <h5 class="card-subtitle mb-2 my-2 fw-bold">About</h5>
                            <p class="card-text text-body-secondary me-3">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
                    <div class="card border-0 py-2" :style="{ width: '', height: '30rem', backgroundColor: '#FCEFD4' }">
                        <div class="card-body ">
                            <h1 class="card-title ">😎</h1>
                            <h5 class="card-subtitle mb-2 fw-bold">Product</h5>
                            <p class="card-text text-body-secondary me-3">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Right Column -->
            <div class="col-lg-4 col-md-12 top float-end">
                <div class="headings">
                    <div class="py-3 fw-bold h1 pe-4 text-end purple-heading " id="heading2">
                        Ahead
                    </div>
                </div>

                <!-- <div class="card rounded-4 p-2" style="width: 100%; height: 40rem;"> -->
                <div class=" rounded-4 pe-4  bg-transparent overflow-auto " style="width: 100%; height: 30rem;">
                    <!-- card  -->
                    <div class="card border-0 py-2 mb-3 rounded-4" :style="{ width: '', backgroundColor: '' }">
                        <div class="card-body">

                            <h5 class="card-subtitle mb-2 my-2 fw-bold">About </h5>
                            <p class="card-text text-body-secondary">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
                    <!-- card  -->
                    <div class="card border-0 py-2 my-3 rounded-4" :style="{ width: '', backgroundColor: '' }">
                        <div class="card-body">

                            <h5 class="card-subtitle mb-2 my-2 fw-bold">About</h5>
                            <p class="card-text text-body-secondary">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
            
                    <!-- card  -->
                    <div class="card border-0 py-2 my-3 rounded-4" :style="{ width: '', backgroundColor: '' }">
                        <div class="card-body">

                            <h5 class="card-subtitle mb-2 my-2 fw-bold">About</h5>
                            <p class="card-text text-body-secondary">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
            
                    <!-- card  -->
                    <div class="card border-0 py-2 my-3 rounded-4" :style="{ width: '', backgroundColor: '' }">
                        <div class="card-body">

                            <h5 class="card-subtitle mb-2 my-2 fw-bold">About</h5>
                            <p class="card-text text-body-secondary">
                                Some quick example text to build on the card title and make up the bulk of the card's
                                content.
                            </p>
                        </div>
                    </div>
            
                  

                </div>
            </div>
        </div>
    </div>
</template>
  

  
<style scoped>


.card {
    border: 0;
}



.card-style1 {
    width: 17rem;
    background-color: #FCEFD4;
}

.card-style2 {
    width: 17rem;
    background-color: #EEEBFE;
}

.card-style3 {
    width: 17rem;
    background-color: #6441EF;
}

.card-style4 {
    width: 17rem;
    background-color: #D9F2FF;

}
.purple-heading{
 color: #6441EF;

}




 
::-webkit-scrollbar {
    width: 6px;
    height: 10px;
    background-color: white;
}


/* Handle on hover */
::-webkit-scrollbar-thumb {
    background: #6341EF;
    border-radius: 10px;

}
@media screen and (min-width:350px) and (max-width: 450px){
.workwithus-main-resp{
    width: 100% !important;
    height: 31rem !important;
}
div#heading1 {
    
    margin-bottom: 30px;
    text-align: center;
}
div#heading2 {
    text-align: center !important;
    margin-top: 30px;
    margin-bottom: 30px;
}
h5.card-subtitle.mb-2.my-2.fw-bold {
    text-align: center;
}
p.card-text.text-body-secondary {
    text-align: center;
}
h5.card-subtitle.mb-2.fw-bold {
    text-align: center;
}
h1.card-title{
    text-align: center;
}

}
@media (min-width: 750px){

 
div#heading1 {
    text-align: center;
    margin: 1.5rem;
}
div#heading2 {
    text-align: center !important;
    margin: 1.5rem;
}
.card.rounded-4.p-2.workwithus-main-resp {
    width: 100% !important;
    text-align: center;
}
}




</style>
<script>

</script>
  