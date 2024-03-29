<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'Contact'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <section>
      <div class="background">
        <div class="navbar">
        </div>
        <h2 div class="con color-white">CONTACT ME</h2>
        <div class="container">
            <form action="ContactView.vue">
              <label div class="go text-gray-200" for="fname">FULL NAME</label>
              <input type="text" id="fname" name="firstname" placeholder="Your Full Name" required="">
          
              <label div class="go text-gray-200" for="email">EMAIL</label>
              <input type="text" id="Email" name="lastname" placeholder="Your Email" required="">
          
              <label class="go text-gray-200" for="subject">MESSAGE</label>
              <textarea id="subject" name="subject" placeholder="Your Message..." class="comment" required=""></textarea>
              <input type="submit" value="Submit">
            </form>
          </div>
        </div>
    </section>
  </MainLayout>
</template>