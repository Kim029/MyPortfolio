<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'About'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <section>
      <div class="background">
        <div class="content-abt">
            <div class="cont-container">
                <img src="https://scontent.fceb3-1.fna.fbcdn.net/v/t1.15752-9/423454983_1105417480495767_8919237847726397319_n.png?_nc_cat=103&ccb=1-7&_nc_sid=8cd0a2&_nc_eui2=AeFGQGlkSkWgPzk_MzsCpkj9e4g1YdaXuQ97iDVh1pe5DxIumulgHb-LpSLlxOqIfvDYfkDqSc-gIPvfoWaZNBYJ&_nc_ohc=a5JOjvDqohkAX-7dp_w&_nc_oc=AQnzh3UvgzadlpKr92ReuUfHi6OppY3vdO1MJ7doZ3dWEticPnVTXQ0FVSAu3GM8NC8&_nc_ht=scontent.fceb3-1.fna&oh=03_AdR68tPkjZZ6088bKwf9YamFOqYQN5YAmWacR6kd49VawQ&oe=660B5E4A">
                <h4>ADDRESS:<br><span>A. Tumulak St., Gun-ob, Lapu-Lapu City</span></h4>
                <h4>MOBILE NUMBER:<br><span>09501743409</span></h4>
            </div>
            <div class="about-me">
                <h1>ABOUT ME</h1>
                <p>
                    Hi, I am Rachiel Ravina, currently taking up a Bachelor of <br>
                    Science in Information Technology at Cordova Public College. <br>
                    I am a person who is interested in the world of web designing, <br>
                    editing photos and photography. I am passionate about improving <br>
                    the lives of others through designs and I am constantly looking <br> 
                    to learn new things everyday. 
                </p>
            </div>
        </div>
    </div>    
  </section>
  </MainLayout>
</template>