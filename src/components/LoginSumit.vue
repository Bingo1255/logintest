<template>
    <span class="login_button">
        <input type="button" />
        <label>Sign In</label>
        <label>Sign Up</label>
    </span>
</template>
<style>
.login_button{
    position: relative;
    display: flex;
    flex: 1;
    overflow: hidden;
}
.login_button input{
    display: block;
    flex: 1;
    width: 0;
    height: 40px;
    border: none;
    border-radius: 2px;
    outline: none;
    background-color: #0760be;

}
.login_button label{
    position: absolute;
    width: 100%;
    height: 100%;
    align-items: center;
    justify-content: center;
    display: flex;
    transition: all .6s ease;

}
</style>