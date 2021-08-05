<template>
    <div class="slider">
        <div class="container">
            <h2 class="slider__title">
                Don’t just take our word for it 
                <svg width="135" height="104" viewBox="0 0 135 104" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M6.07002 53.16L39.57 0H64.42L43.04 44.78C48.24 46.7 52.67 50.27 56.34 55.47C59.9793 60.6184 61.8974 66.7857 61.82 73.09C61.82 81.56 58.74 88.89 52.58 95.04C49.7708 97.9363 46.3975 100.226 42.6686 101.767C38.9397 103.308 34.9343 104.068 30.9 104C22.43 104 15.1 101.02 8.95002 95.04C6.06906 92.1656 3.79288 88.7435 2.25573 84.9753C0.718585 81.2072 -0.0483978 77.1693 2.13226e-05 73.1C2.13226e-05 66.17 2.02002 59.52 6.07002 53.17V53.16ZM75.97 53.16L109.5 0H134.34L112.97 44.78C118.17 46.7 122.6 50.27 126.25 55.47C129.897 60.6157 131.822 66.7834 131.75 73.09C131.75 81.56 128.66 88.89 122.5 95.04C119.692 97.935 116.32 100.224 112.593 101.765C108.866 103.306 104.863 104.067 100.83 104C92.36 104 85.04 101.02 78.88 95.04C75.9936 92.1682 73.7119 88.7471 72.1696 84.9788C70.6272 81.2105 69.8555 77.1714 69.9 73.1C69.9 66.17 71.92 59.52 75.97 53.17V53.16Z" fill="#FFF7E0"/>
                </svg>
            </h2>
            <div class="slider__slider">
                <VueSlickCarousel v-bind="settings">
                    <h2 class="slider__info">
                        “I've been using Superpeer with about 10-12 calls per week, and so far the experience has been flawless.”
                    </h2>
                    <h2 class="slider__info">
                        “I've been using Superpeer with about 10-12 calls per week, and so far the experience has been flawless.”
                    </h2>
                    <h2 class="slider__info">
                        “I've been using Superpeer with about 10-12 calls per week, and so far the experience has been flawless.”
                    </h2>
                </VueSlickCarousel>
                <button class="btn arrow-left">
                    <svg width="54" height="54" viewBox="0 0 54 54" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="54" height="54" rx="27" fill="#EEEEEE"/>
                        <path d="M25.614 20.9248L21.528 25.8298H34.875C35.1734 25.8298 35.4595 25.9484 35.6705 26.1593C35.8815 26.3703 36 26.6565 36 26.9548C36 27.2532 35.8815 27.5393 35.6705 27.7503C35.4595 27.9613 35.1734 28.0798 34.875 28.0798H21.5262L25.614 32.9848C25.7128 33.0977 25.788 33.2292 25.8352 33.3716C25.8824 33.514 25.9006 33.6644 25.8888 33.814C25.877 33.9635 25.8354 34.1092 25.7665 34.2424C25.6976 34.3757 25.6027 34.4938 25.4875 34.5898C25.3723 34.6858 25.239 34.7579 25.0955 34.8016C24.952 34.8454 24.8012 34.86 24.652 34.8446C24.5028 34.8293 24.3581 34.7842 24.2266 34.7121C24.095 34.64 23.9792 34.5423 23.886 34.4248L18.261 27.6748C18.2304 27.6388 18.2106 27.5974 18.189 27.5578C18.1726 27.5228 18.1546 27.4886 18.135 27.4552C18.1152 27.4264 18.0954 27.3958 18.081 27.3616C18.0297 27.2333 18.0028 27.0966 18.0018 26.9584V26.9566L18 26.9548V26.9512C18 26.8126 18.0306 26.6776 18.0828 26.548C18.0954 26.512 18.1152 26.4832 18.1332 26.4544L18.162 26.4076L18.1908 26.3536C18.2106 26.3122 18.2304 26.2708 18.261 26.2348L23.886 19.4848C23.9792 19.3673 24.095 19.2696 24.2266 19.1975C24.3581 19.1254 24.5028 19.0804 24.652 19.065C24.8012 19.0496 24.952 19.0643 25.0955 19.108C25.239 19.1518 25.3723 19.2238 25.4875 19.3198C25.6027 19.4159 25.6976 19.534 25.7665 19.6672C25.8354 19.8005 25.877 19.9461 25.8888 20.0957C25.9006 20.2452 25.8824 20.3956 25.8352 20.538C25.788 20.6804 25.7128 20.8119 25.614 20.9248Z" fill="black"/>
                    </svg>
                </button>
                <button  class="btn arrow-right">
                    <img src="../assets/arr.png" alt="">         
                </button>
            </div>
        </div>
    </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name : "Slider",
    components : {
        VueSlickCarousel 
    },
    data(){
        return{
            settings : {
            "dots": false,
            "dotsClass": "slick-dots custom-dot-class",
            "edgeFriction": 0.35,
            "infinite": true,
            "speed": 500,
            "slidesToShow": 1,
            "slidesToScroll": 1,
            "autoplay": true,
            "prevArrow": ".arrow-left",
            "nextArrow": ".arrow-right",
            }
        }
    }
}
</script>

<style lang="scss">
.slider{
    background: linear-gradient(180deg, #FFFAEC 0%, rgba(255, 255, 255, 0) 100%);
    background-image: url('../assets/slb.png');
    background-repeat: no-repeat;
    background-size: contain;
    background-position: bottom;
    padding: 120px 0;
    &__title{
        font-size: 48px;
        line-height: 53px;
        text-align: center;
        letter-spacing: 1px;
        color: #222222;
        position: relative;
        svg{
            position: absolute;
            top: 50%;
            z-index: -1;
            right: 50%;
            transform: translate(50%, -50%);
        }
    }
    &__info{
        font-size: 32px;
        line-height: 40px;
        text-align: center;
        color: #222222;
        font-weight: 400;
    }
    .slick-slider{
        margin: 86px 0;
    }
    &__slider{
        position: relative;
        width: 90%;
        margin: auto;
    }
    .arrow-left{
        position: absolute;
        top: 50%;
        transform: translateY(-50%);  
        left: -72px;
    }
    .arrow-right{
        position: absolute;
        right: -72px;
        top: 50%;
        transform: translateY(-50%);    
    }

}

@media (max-width:776px) {
    .slider{
        &__info{
            font-size: 20px;
            line-height: 32px;
        }
        &__title{
            font-size: 36px;
        }
        &__slider{
            width: 80%;
        }
        .arrow-left{
            left: -56px;
            svg{
                width: 60%;
            }
        }
        .arrow-right{
            right: -56px;
            img{
                width: 60%;
            }
        }
    }
}
</style>