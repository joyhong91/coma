<template>
    <div class="intro_section">
        <div class="img_wrapper fst">
            <img src="~/assets/imgs/intro/slide_1_v2.jpg" class="intro_img img1"/>
            <a class="btn_next" href="#" data-dir="2">
               <img src="~/assets/imgs/icon/intro_arr.png" class="" />
               <span class="txt_next"> 옆으로 넘겨보세요!</span>     
            </a>
        </div> 
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_2.jpg" class="intro_img img2"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="1">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="3">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div> 
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_3.jpg" class="intro_img img3"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="2">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="4">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div> 
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_4.jpg" class="intro_img img4"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="3">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="5">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div>
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_5.jpg" class="intro_img img5"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="4">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="6">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div>  
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_6_v2.jpg" class="intro_img img6"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="5">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="7">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div> 
        <div class="img_wrapper hide">
            <img src="~/assets/imgs/intro/slide_7.jpg" class="intro_img img7"/>
            <div class="btn_wrapper">
                <a class="btn_prev" href="#" data-dir="6">
                <img src="~/assets/imgs/icon/intro_arr_left_bl.png" class=""/>
                </a>
                <a class="btn_next" href="#" data-dir="1">
                <img src="~/assets/imgs/icon/intro_arr_bl.png" class=""/>
                </a>
            </div>
        </div> 

        <script>
            $('.btn_next, .btn_prev').on('click', function(){
                var dir = $(this).data('dir');
                console.log(dir);
                var $imgWrappers = $('.intro_section .img_wrapper');

                $imgWrappers.hide().eq(parseInt(dir) - 1).show();
            })
        </script>
    </div>
   
</template>

<style scoped>
.hide {
    display: none;
}
.intro_section {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #000;
    height: 100vh;
}

.img_wrapper {
    position: relative;
    width: 100%;
}
.intro_img{
    width: 100%;
}

.img_wrapper.fst .btn_next {
    position: absolute;
    bottom: 40%;
    right: 4%;
}

.img_wrapper:not(.fst) .btn_wrapper{
    position: absolute;
    bottom: 45%;
    width: 100%;
}

.img_wrapper:not(.fst) .btn_prev img,
.img_wrapper:not(.fst) .btn_next img{
    width: 6%;
}

.btn_prev img{
    float: left;
}

.btn_next img,
.btn_prev img{
    max-width: 23%;
    display: block;
    margin-left: auto;
    margin-bottom: 3px;
    -webkit-animation:blink 0.7s ease-in-out infinite alternate;
    -moz-animation:blink 0.7s ease-in-out infinite alternate;
    animation:blink 0.7s ease-in-out infinite alternate;
}

@-webkit-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@-moz-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}


.btn_next span{
    font-size: 0.9rem;
    color: #fff;
    float: right;
}

.btn_next .ico_arr {
    background: url(/assets/imgs/icon/intro_arr.png);
}
.ico_arr {

}
</style>

