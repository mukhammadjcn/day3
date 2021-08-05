<template>
  <div class="home">
      <Header />
      <intro />
      <communty :people="users"/>
      <super />
      <features />
      <slider />
      <series />
      <animi />
      <Footer />
  </div>
</template>

<script>
import Animi from '../components/Animi.vue'
import Communty from '../components/Communty.vue'
import Features from '../components/Features.vue'
import Footer from '../components/Footer.vue'
import Header from '../components/Header.vue'
import Intro from '../components/Intro.vue'
import Series from '../components/Series.vue'
import Slider from '../components/Slider.vue'
import Super from '../components/Super.vue'


export default {
  name: 'Home',
  components: {
    Header,
    Intro,
    Communty,
    Super,
    Features,
    Slider,
    Series,
    Animi,
    Footer
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
                    status : "Coming Soon",
                    followed: false
                },
                {
                    id : 2,
                    userBg : require("../assets/users/user2.png"),
                    userAvatar : require("../assets/users/user2mini.png"),
                    userName : "Thomas Hopkins",
                    userTitle: "Paid Marketing",
                    userArticle : "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    userDate: "August 6, 2021",
                    label : "ENROLL",
                    followed: false
                },
                {
                    id : 3,
                    userBg : require("../assets/users/user3.png"),
                    userAvatar : require("../assets/users/user3mini.png"),
                    userName : "Alice Johnson",
                    userTitle: "Find Your True Love, your TwinFlame®",
                    userArticle : "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    userDate: "July 26, 2021",
                    label : "ENROLL",
                    followed: false
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
                    status : "Coming Soon",
                    followed: false
                },
                {
                    id : 5,
                    userBg : require("../assets/users/user5.png"),
                    userAvatar : require("../assets/users/user5mini.png"),
                    userName : "Jason Akel",
                    userTitle: "Self-Hypnosis and HypnoTherapy Adventures",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "July 24, 2021",
                    label : "ENROLL",
                    followed: false
                },
                {
                    id : 6,
                    userBg : require("../assets/users/user6.png"),
                    userAvatar : require("../assets/users/user6mini.png"),
                    userTitle: "Movement Building",
                    userName : "Tristan Pollock",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "July 28, 2021",
                    label : "ENROLL",
                    followed: false
                },
                {
                    id : 7,
                    userBg : require("../assets/users/user7.png"),
                    userAvatar : require("../assets/users/user7mini.png"),
                    userTitle: "Pitch Deck Examples & How to Class",
                    userName : "Jose Caya",
                    userArticle : "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    userDate: "August 6, 2021",
                    label : "NOTIFY ME",
                    followed: false
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
                    status : "Coming Soon",
                    followed: false
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
                    status : "Coming Soon",
                    followed: false
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
                    followed: false
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
  z-index: 2;
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

@media (max-width:600px) {
  .home{
    overflow: hidden;
  }
  .contactBtn {
        position: fixed;
        bottom: 10px;
        right: 20px;
        svg{
            width: 80%;
        }
  }
}
</style>
