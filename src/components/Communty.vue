<template>
    <div class="communty">
        <div class="container">
            <h2 class="title">See what magic our community is creating</h2>
            <p class="info">Explore these examples of Series, created by our Superpeers, and reserve your spot today</p>
            <div class="row users">
                <div  class="user" v-for="(item, index) in people" :key="index">
                    <div>
                          <div class="user__images">
                        <img  class="userBg" :src="item.userBg" alt="">
                        <img class="userAvatar" :src="item.userAvatar" alt="">
                        <span class="user__status" v-if="item.status">{{item.status}}</span>
                    </div>
                    <div class="user__detail">
                        <h2 class="user__title">{{item.userTitle}}</h2>
                        <span class="user__name">{{item.userName}}</span>
                        <p class="minInfo">{{item.userArticle}}</p>
                        <div class="row">
                            <span class="user__startDate minInfo">Starts : <span>{{item.userDate}}</span></span>
                            <button class="btn tr" @click="toggle(item)">{{item.followed ? item.label : "FOLLOWED"}}</button>
                        </div>
                    </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : "Communty",
    data(){
        return{
            isBtn : true,
        }
    },
    props : {
        people : {
            type : Array,
            default : () => {[]}
        }
    },
    methods :{
        toggle(item){
            item.followed = !item.followed
        }
    }
}
</script>

<style lang="scss">
.communty{
    padding: 180px 0;
    background: linear-gradient(180deg, #FFF7E0 0%, #FFFFFF 100%);
    .title{
        width: 60%;
        margin: auto;
        text-align: center;
    }
    .info{
        width: 60%;
        margin: auto;
        margin-top: 36px;
    }
    .users{
        margin: 64px 0;
        gap: 120px;
        flex-wrap: wrap;
    }
}
.user{
    flex-basis: 40%;
    text-align: center;
    &__images{
        position: relative;
        .userBg{
            width: 100%;
            border-radius: 14px;
        }
        .userAvatar{
            position: absolute;
            bottom: 0;
            left: 50%;
            border: 8px solid white;
            transform: translate(-50%, 50%);
            border-radius: 50%;
        }
    }
    &__title{
        margin: 48px 0 12px;
        font-weight: bold;
        font-size: 22px;
        line-height: 29px;
        color: #222222;
    }
    .minInfo{
        margin: 20px 0;
    }
    &__startDate{
        color: #98A3B6 !important;
        span{
            color: black;
        }
    }
    &__detail{
        .row{
            gap: 24px;
            .btn{
                padding: 12px 24px;
                background: #FFEDC2;
                border-radius: 8px;
                &:hover{
                    background: antiquewhite;
                }
            }
        }
    }
    &__status{
        position: absolute;
        top: 20px;
        right: 20px;
        padding: 12px;
        background: #FFEDC2;
        border-radius: 30px;
        font-size: 12px;
        line-height: 16px;
        text-align: center;
        text-transform: uppercase;
        color: #665000;
    }
}

@media(max-width:776px){
    .communty{
        padding: 36px 0;
        .users{
            flex-direction: column;
            gap: 56px;
        }
        .user__status{
            top: 10px;
            right: 10px;
            padding: 8px;
            font-size: 10px;
            line-height: initial;
        }
        .info{
            width: 100%;
        }
    }
}
</style>