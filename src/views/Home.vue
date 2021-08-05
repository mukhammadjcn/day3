<template>
  <div class="home">
      <Header/>
      <intro/>
      <communty :persons="users"/>
      <button class="contactBtn btn">
        <svg width="72" height="72" viewBox="0 0 72 72" fill="none" xmlns="http://www.w3.org/2000/svg">
          <g filter="url(#filter0_d)">
          <rect x="6" y="5" width="60" height="60" rx="5" fill="#FFD338"/>
          </g>
          <path d="M50 51C50 51 45.286 49.145 41.473 47.66H25.437C23.54 47.66 22 46.026 22 44.013V22.644C22 20.633 23.54 19 25.437 19H46.562C48.46 19 49.999 20.632 49.999 22.645V41.049H50V51ZM45.861 39.018C45.7861 38.9219 45.6921 38.8423 45.5848 38.7844C45.4776 38.7266 45.3595 38.6916 45.2381 38.6817C45.1166 38.6718 44.9944 38.6873 44.8792 38.7271C44.7641 38.7669 44.6584 38.8302 44.569 38.913C44.539 38.939 41.554 41.594 35.999 41.594C30.513 41.594 27.482 38.958 27.428 38.91C27.3385 38.8277 27.2329 38.7648 27.1178 38.7253C27.0027 38.6859 26.8808 38.6707 26.7595 38.6807C26.6383 38.6908 26.5205 38.7258 26.4135 38.7837C26.3066 38.8416 26.2127 38.921 26.138 39.017C25.9779 39.2167 25.8997 39.4698 25.919 39.725C25.9359 39.9789 26.0498 40.2167 26.237 40.389C26.379 40.517 29.774 43.539 35.999 43.539C42.225 43.539 45.62 40.517 45.762 40.389C45.9489 40.2165 46.0624 39.9788 46.079 39.725C46.0984 39.4702 46.0205 39.2176 45.861 39.018Z" fill="black" fill-opacity="0.71"/>
          <defs>
          <filter id="filter0_d" x="0" y="0" width="72" height="72" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
          <feFlood flood-opacity="0" result="BackgroundImageFix"/>
          <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
          <feOffset dy="1"/>
          <feGaussianBlur stdDeviation="3"/>
          <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.06 0"/>
          <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
          <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
          </filter>
          </defs>
        </svg>
      </button>
  </div>
</template>

<script>
import Communty from '../components/Communty.vue'
import Header from '../components/Header.vue'
import Intro from '../components/Intro.vue'


export default {
  name: 'Home',
  components: {
    Header,
    Intro,
    Communty
  },
  data(){
    return{
      users : [
                {
                    id : 1,
                    userBg : require("../assets/users/user1.png"),
                    userAvatar : require("../assets/users/user1mini.png"),
                    userName : "Dawn Dickson",
                    userTitle: "Masterclass on Fundraising Strategies",
                    userArticle : "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    userDate: "September 9, 2021",
                    label : "ENROLL",
                    status : "Coming Soon"
                },
                {
                    id : 2,
                    userBg : require("../assets/users/user2.png"),
                    userAvatar : require("../assets/users/user2mini.png"),
                    userName : "Thomas Hopkins",
                    userTitle: "Paid Marketing",
                    userArticle : "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    userDate: "August 6, 2021",
                    label : "ENROLL"
                },
                {
                    id : 3,
                    userBg : require("../assets/users/user3.png"),
                    userAvatar : require("../assets/users/user3mini.png"),
                    userName : "Alice Johnson",
                    userTitle: "Find Your True Love, your TwinFlame®",
                    userArticle : "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    userDate: "July 26, 2021",
                    label : "ENROLL"
                },
                {
                    id : 4,
                    userBg : require("../assets/users/user4.png"),
                    userAvatar : require("../assets/users/user4mini.png"),
                    userName : "Mark Wahlbeck",
                    userTitle: "Fiction Writing For Absolute Beginners: How To Publish Your First Story",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 2, 2021",
                    label : "ENROLL",
                    status : "Coming Soon"
                },
                {
                    id : 5,
                    userBg : require("../assets/users/user5.png"),
                    userAvatar : require("../assets/users/user5mini.png"),
                    userName : "Jason Akel",
                    userTitle: "Self-Hypnosis and HypnoTherapy Adventures",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "July 24, 2021",
                    label : "ENROLL"
                },
                {
                    id : 6,
                    userBg : require("../assets/users/user6.png"),
                    userAvatar : require("../assets/users/user6mini.png"),
                    userTitle: "Movement Building",
                    userName : "Tristan Pollock",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "July 28, 2021",
                    label : "ENROLL"
                },
                {
                    id : 7,
                    userBg : require("../assets/users/user7.png"),
                    userAvatar : require("../assets/users/user7mini.png"),
                    userTitle: "Pitch Deck Examples & How to Class",
                    userName : "Jose Caya",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 6, 2021",
                    label : "NOTIFY ME"
                },
                {
                    id : 8,
                    userBg : require("../assets/users/user8.png"),
                    userAvatar : require("../assets/users/user8mini.png"),
                    userTitle: "Starting your Business",
                    userName : "Devrim Yasar",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 29, 2021",
                    label : "NOTIFY ME",
                    status : "Coming Soon"
                },
                {
                    id : 9,
                    userBg : require("../assets/users/user9.png"),
                    userAvatar : require("../assets/users/user9mini.png"),
                    userTitle: "Public Speaking",
                    userName : "Armagan Amcalar",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 23, 2021",
                    label : "NOTIFY ME",
                    status : "Coming Soon"
                },
                {
                    id : 10,
                    userBg : require("../assets/users/user10.png"),
                    userAvatar : require("../assets/users/user10mini.png"),
                    userTitle: "You can’t Entrepreneur without PM",
                    userName : "Jasmine Lawrence",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 25, 2021",
                    label : "NOTIFY ME",
                },
                
            ]
    }
  }
}
    
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style-type: none;
  text-decoration-line: none;
  font-family: 'Roboto', sans-serif;
}
.container{
  max-width: 1080px;
  margin: auto;
}
.btn{
  border: none;
  outline: none;
  background: none;
}
.row{
  display: flex;
  align-items: center;
  justify-content: center;
}
.title{
  font-weight: bold;
  font-size: 48px;
  line-height: 53px;
  letter-spacing: 1px;
  color: #222222;
}
.minInfo{
  font-size: 16px;
  line-height: 22px;
  text-align: center;
  color: #555555;
}
.info{
  font-size: 18px;
  line-height: 25px;
  text-align: center;
  color: #222222;
}
.bigInfo{
  font-size: 22px;
  line-height: 29px;
  text-align: center;
  color: #555555;
}
.contactBtn{
  position: fixed;
  bottom: 40px;
  right: 40px;
}

@media(max-width:1180px){
    .container{
        max-width: 90%;
    }
    .title{
        font-size: 24px;
        line-height: 36px;
        width: 100% !important;
    }
}
</style>
