<template>
    <div class="contact" id="contact">
        <div>
            <h2>Contact Me</h2>
            <form ref="form" @submit.prevent="sendEmail">
                <aside>
                    <input type="text" name="name" v-model="name" placeholder="Your Name">
                    <input v-if="alert" class="email-alert" type="email" name="email" v-model="email" placeholder="Your Email">
                    <input v-else class="email" type="email" name="email" v-model="email" placeholder="Your Email">
                </aside>
                <textarea v-if="alert" class="message-alert" name="message" v-model="message" cols="30" rows="10" placeholder="SENT!"></textarea>
                <textarea v-else class="message" name="message" v-model="message" cols="30" rows="10" placeholder="Message"></textarea>
                <input type="submit" value="Send">
            </form>
        </div>
    </div>
</template>

<script>

import emailjs from 'emailjs-com'

export default{
    data(){
        return{
            name:'',
            email:'',
            message:'',
            alert: false
        }
    },
    methods:{
        sendEmail(e){
            try{
                emailjs.sendForm('service_71cov0y','template_k9o9xcv',e.target,'HOPIlZBeW7ASwXYTh',{
                name:this.name,
                email:this.email,
                message:this.message
                })
                this.alert = true;
                console.log("Success!")
            }catch(error){
                console.log(error)
            }
            
            this.name = '',
            this.email = '',
            this.message = ''
            
        }
        
    }
}
</script>

<style>
    .contact{
        margin-top: 10vh;
        background-color: whitesmoke;
        opacity: .9;
        border-radius: 100px 1px 100px 1px / 120px;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 5vh 0;
    }

    .contact > div{
        width: 80%;
        height: 80%;
    }

    .contact h2{
        background-color: #0F0F27;
        padding: 1vh 1vh;
        color: white;
        border-radius: 100px 1px 100px 1px / 120px;
        margin-bottom: 2vh;
    }

    .contact aside{
        display: flex;
        gap: 5vh;
        padding-bottom: 2vh;
    }

    input[type=text]{
        width: 30%;
        padding: 1vh 3vh;
        border: 1px solid #0F0F27;
        border-radius: 5px;
        font-size: 1rem;

    }

    .email{
        width: 60%;
        padding: 1vh 3vh;
        border: 1px solid #0F0F27;
        border-radius: 5px;
        font-size: 1rem;
        background:linear-gradient(130deg,whitesmoke,whitesmoke,#0F0F27);

    }

    .email-alert{
        width: 60%;
        padding: 1vh 3vh;
        border: 1px solid #0F0F27;
        border-radius: 5px;
        font-size: 1rem;
        background:linear-gradient(130deg,whitesmoke,whitesmoke,#0cd613);

    }

    input[type=submit]{
        width: 20%;
        padding: 1vh 3vh;
        background-color: #0F0F27;
        color: white;
        border-radius: 100px 1px 100px 1px / 120px;
        font-weight: 600;
        font-size: .9rem;
    }

    ::placeholder{
        color: #0F0F27;
    }

    input[type=submit]:hover{
        cursor: pointer;
        background-color: #FC2A30;
        transition: .3s;
        border-radius: 1px 100px / 120px;
    }

    .message{
        resize: none;
        width: 97%;
        height: 20vh;
        font-size: 1rem;
        margin-bottom: 1vh;
        border: 1px solid #0F0F27;
        border-radius: 5px;
        padding: 2vh;
        background:linear-gradient(130deg,whitesmoke,whitesmoke,#0F0F27);
    }

    .message-alert{
        resize: none;
        width: 97%;
        height: 20vh;
        font-size: 1rem;
        margin-bottom: 1vh;
        border: 1px solid #0F0F27;
        border-radius: 5px;
        padding: 2vh;
        background:linear-gradient(130deg,whitesmoke,whitesmoke,#0cd613);
    }
</style>