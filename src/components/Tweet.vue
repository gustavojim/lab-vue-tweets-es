<template>
    <div class="tweet">

        <!-- Creo el enlace a los componenentes  -->

        <ProfileImage :src="props.tweet.user.image"></ProfileImage>
        
        <div class="body">

            <div class="top">
                <User :users="props.tweet.user.name" :handle="props.tweet.user.handle"></User> 
            </div>

        <!-- Creo en enlace a User -->



        <!-- Creo en enlace a TimeStamp -->

            <TimeStamp></TimeStamp>

        <!-- Creo en enlace a Message -->

            <Message :mensaje="props.tweet.message"></Message>

        <!-- Creo en enlace a Actions -->

        <Actions></Actions>
        </div>
        <i class="fas fa-ellipsis-h"></i>
    </div>


        <!-- <img src="https://i.imgur.com/9yw1Fyw.jpg" class="profile" alt="profile" />
        <div class="body">
            <div class="top">
                <span class="user">
                    <span class="name">Ironhack</span>
                    <span class="handle">@ironhack</span>
                </span>

                <span class="timestamp">Nov 30, 2020</span>
            </div>

            <p class="message">
                On December 7th, we will be hosting a #webinar that will introduce you
                to #SQL! Are you ready? 🚀
            </p>

            <div class="actions"> -->
                <!-- Font Awesome icons -->
                <!-- <i class="far fa-comment"></i>
                <i class="fas fa-retweet"></i>
                <i class="far fa-heart"></i>
                <i class="fas fa-share"></i>
            </div> -->
        <!-- </div> -->

   
</template>
  
<style scoped>
a {
    color: #42b983;
}
</style>

<!-- Importo todas las props de los componentes -->

<script setup>
    import { defineProps } from 'vue';
    import ProfileImage from './ProfileImage.vue';
    import Actions from './Actions.vue';
    import Message from './Message.vue';
    import TimeStamp from './TimeStamp.vue';
    import User from './User.vue';
    const props = defineProps(['tweet']);

</script>