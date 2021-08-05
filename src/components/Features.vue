<template>
    <div class="features">
        <div class="container">
            <h1 class="title">What can Superpeer dofor you?</h1>
            <p class="info">Turn your audience into loyal, paying followers with our seamless video experience and subscriber management tools.</p>
            <div class="row">
                <div class="feature">
                    <img src="../assets/feature1.png" alt="">
                    <h3 class="info">Engage with your audience</h3>
                    <p class="minInfo">Connect with your subscribers through interactive livestreams, 1:1s, and our newest feature, Series.</p>
                </div>
                <div class="feature">
                    <img src="../assets/feature2.png" alt="">
                    <h3 class="info">Manage easier</h3>
                    <p class="minInfo">We take care of scheduling, payments, and protecting your privacy, so that you don’t have to.</p>
                </div>
                <div class="feature">
                    <img src="../assets/feature3.png" alt="">
                    <h3 class="info">Earn, your way</h3>
                    <p class="minInfo">Set your own rates and earn revenue through weekly livestreams, channel subscriptions, and even donations.</p>
                </div>
            </div>
            <button class="btn">All Features</button>
        </div>
    </div>
</template>

<script>
export default {
    name : "Features"
}
</script>

<style lang="scss">
.features{
    padding: 120px 0;
    background: linear-gradient(180deg, #FDE6E6 0%, #FFFFFF 100%);
    text-align: center;
    .row{
        padding: 124px 0;
        gap: 86px;
        justify-content: space-between;
    }
    .info{
        width: 80%;
        margin: 28px auto;
    }
    .feature{
        .info{
            margin: 24px 0 12px;
            width: 100%;
            font-weight: 500;
        }
    }
    .btn{
        padding: 12px 24px;
        background: #FFEDC2;
        border-radius: 8px;
        font-size: 16px;
        line-height: 22px;
    }
}

@media (max-width:776px) {
    .features {
        .row{
            flex-wrap: wrap;
        }
    }
}
</style>