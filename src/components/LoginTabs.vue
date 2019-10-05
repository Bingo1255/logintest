<template>
    <ul class="login_tabs">
        <li><span>Sign up</span></li>
        <li class="login_tabs_s">or</li>
        <li><span>Sign in</span></li>
    </ul>
</template>
<style>
    .login_tabs{
        display: flex;
        padding: 0 34px;
    }
    .login_tabs li{
        display: flex;
        padding: 10px;
        flex: 1;
        justify-content: space-around;
        /* 设置弹性盒子元素在主轴（横轴）的对齐方式。 */
        align-items: center;
        /* 设置弹性盒子元素在垂直方向上（纵轴）的对齐方式 */
        transition: all .6 ease;
    }
    .login_tabs span{
        display: block;
        border: 1px solid white;
        padding: 4px 10px;
        border-radius: 3px;
        text-align: center;
        transition: all .6 ease;

    }
    .login_tabs .login_tabs_s{
        justify-content: center;
        transition-duration: .55s;
        /* transition-duration 属性规定完成过渡效果需要花费的时间 */
        transition-delay: .05s;
    }
    .login_tabs_s {
        font-size: 12px;
    }
    .login_tabs_s::before,
    .login_tabs_s::after{
        content: '-';
    }
    .login_signup .login_tabs li:first-child{
        transition-duration: .5s;
        transition-delay: .1s;
        transform: translateX(100%) scale(1.5);
    }
    .login_signup .login_tabs li:first-child span{
        border-color: transparent;
    }
    .login_signup .login_tabs li:last-child{
        transform: scale(0.6);
        opacity: 0.4;
    }
    .login_signup .login_tabs_s{
        transform: translateX(58%);
        opacity: 0.8;
    }
    .login_signin .login_tabs li:last-child{
        transition-duration: .5s;
        transition-delay: .1s;
        transform: translateX(-100%) scale(1.5);
    }
    .login_signin .login_tabs li:last-child span{
        border-color: transparent;
    }
    .login_signin .login_tabs li:first-child{
        transform: scale(0.6);
        opacity: 0.4;
    }
    .login_signin .login_tabs_s{
        transform: translateX(-58%);
        opacity: 0.8;
    }
</style>