<template>
    <div class="login" :class="{ login_signin: isSignIn,login_signup:isSignUp}">
        <LoginTabs @click.native="switchState" />
        <LoginForm />
    </div>
</template>
<script>
import LoginTabs from './LoginTabs'
import LoginForm from './LoginForm'
export default {
    components:{
        LoginTabs,
        LoginForm
    },
    data(){
        return{
            state:1
        }
    },
    computed:{
        isSignIn(){
            return this.state===1
            // return true or false
        },
        isSignUp(){
            return this.state===2
        }
    },
    methods:{
        switchState(){
            this.state = this.state === 1?2:1
            
        }
    }
}
</script>
<style scoped>
    .login{
        width: 100%;
        color: white;
        font-size: 14px;

    }
</style>