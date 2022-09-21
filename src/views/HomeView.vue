<template>
  <div class="home">

      <NavBar></NavBar>

      <div class="home_content_container">
        <div class="home_content">

          <h1>Unlimited movies, TV <br> shows, and more.</h1>
          <p>Watch anywhere. Cancel anytime.</p>
          
          <p>Ready to watch? Enter your email to create or restart your membership.</p>
          <div class="search_input">
            <input type="email" placeholder="Email address">
            <button class="">GET Started ></button>
          </div>
    
        </div>
      </div>
  </div>

  <div class="line"></div>


  <div class="home_sectionA  container">
    <div class="home_Abox1">
      <h1>Enjoy on your TV.</h1>
      <p>Watch on Smart TVs, Playstation, Xbox, Chromecast, Apple TV, Blu-ray players, and more.</p>
    </div>
    <div class="home_Abox2">
      <img src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/tv.png" alt="">
    </div>
  </div>

  <div class="line"></div>

  
  <div class="home_sectionB container">
    <div class="home_Bbox1">
      <img src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/mobile-0819.jpg" alt="">
    </div>
    <div class="home_Bbox2">
      <h1>Download your shows <br> to watch offline.</h1>
      <p>Save your favorites easily and always have something to watch.</p>
    </div>
  </div>

  <div class="line"></div>

  <div class="home_sectionC container ">
    <h1>Watch everywhere.</h1>
    <p>Stream unlimited movies and TV shows on <br> your phone, tablet, laptop, and TV.</p>
  </div>

  <div class="line"></div>

  <div class="home_sectionD container">
    <div class="home_Dbox1">
      <img src="https://bit.ly/3SjUYgz" alt="">
    </div>
    <div class="home_Dbox1">
      <h1>Create profiles for kids.</h1>
      <p>Send kids on adventures with their favorite characters in a space made just for them—free with your membership.</p>
    </div>
  </div>

  <div class="line"></div>

  <HomeQuestion></HomeQuestion>

  <div class="line"></div>

  <div class="home_footer container">
    <div class="home_Fheader">
      <router-link to="">Questions? Contact us.</router-link>
    </div>
    <div class="home_Fbox">
      <div class="home_Fcol_1">
        <router-link to="">FAQ</router-link>
        <router-link to="">Investor Relations</router-link>
        <router-link to="">Privacy</router-link>
        <router-link to="">Speed Test</router-link>
      </div>
      <div class="home_Fcol_2">
        <router-link to="">Help Center</router-link>
        <router-link to="">Jobs</router-link>
        <router-link to="">Cookie Preferences</router-link>
        <router-link to="">Legal Notices</router-link>
      </div>
      <div class="home_Fcol_3">
        <router-link to="">Account</router-link>
        <router-link to="">Ways to Watch</router-link>
        <router-link to="">Corporate Information</router-link>
        <router-link to="">Only on Netflix</router-link>
      </div>
      <div class="home_Fcol_4">
         <router-link to="">Media Center</router-link>
        <router-link to="">Terms of Use</router-link>
        <router-link to="">Contact Us</router-link>
      </div>
    </div>

     <div class="home_Ffoot">
      <router-link to="">Netflix Myanmar (Burma)</router-link>
    </div>

  </div>

</template>

<script>
import HomeQuestion from '../components/HomeQuestion'
import NavBar from '../components/NavBar'
// @ is an alias to /src


export default {
  components: {
    HomeQuestion, NavBar },
  
}
</script>

<style>







  .home{
    width: 100%;
    height: 100vh;
    text-align: center;
    background: radial-gradient(gray,black);
    background-image: url("../assets/netflix_home_background.png");
    box-shadow:inset -100px -150px 500px black,
                inset 50px 50px 300px black;
    color: #fff;
  }
  .line{
    border-top: 8px solid #222222;
  }
  .home .home_content_container{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 100px;
  }

  .home .home_content h1{
    font-size: 50px ;
    font-weight: bold !important;
  }  
  .home .home_content p{
    font-size: 20px ;
  }  
  .home .home_content .search_input{
    width: 100%;
    max-width: 750px;
    height: 65px;
    background-color: #fff;
    margin: 0 auto;
    overflow: hidden;
  }
  .home .home_content .search_input input{
    width: 70%;
    height: 70px;
    padding: 10px 20px;
    font-size: 20px;
  }
  .home .home_content .search_input button{
    /* width: 20%; */
    height: 100%;
    font-size: 25px;
    padding:10px 15px;
    background-color: #F40612;
    color: #fff;
    border: none;
    outline: none;
  }

  /* home sectionA */

  .home_sectionA{
    display: flex;
    align-items: center;
    background-color: black;
    color: #fff;
  }
  .home_sectionA {
    text-align: left;
  }
  .home_sectionA .home_Abox1{
    width: 50%;
    padding:10px;
  }
   
  .home_sectionA h1{
    font-size: 55px;
    font-weight: bold;
    margin-bottom: 20px;
  }
   .home_sectionA p{
    font-size: 25px;
  }
  .home_sectionA .home_Abox2{
    width: 50%;
    padding: 30px;
  }
  .home_sectionA .home_Abox2 img{
    width: 100%;
  }

  /* home sectionB */

  .home_sectionB{
    width: 100%;
    display: flex;
    align-items: center;
    background-color: black;
    color: #fff;
    padding: 20px 10px;
  }
  .home_sectionB .home_Bbox1{
    width: 50%;
    padding: 10px;
    padding-right:100px ;
  }
   .home_sectionB .home_Bbox1 img{
     width: 100%;
  }
  .home_sectionB .home_Bbox2{
    width: 50%;
    padding: 10px;
  }
  .home_sectionB .home_Bbox2 h1{
    font-size: 50px;
    font-weight: bold;
  }
  .home_sectionB .home_Bbox2 p{
    font-size: 25px;
  }

  /* home sectionC */

  .home_sectionC{
    background-color: black;
    color: #fff;
    padding: 40px 20px;
  }
    .home_sectionC h1{
    font-size: 50px;
    font-weight: bold;
  }
  .home_sectionC p{
    font-size: 25px;
  }

  /* home sectionD */

  .home_sectionD{
    width: 100%;
    display: flex;
    align-items: center;
    padding: 20px 0;
    color: #fff;
  }
  .home_sectionD .home_Dbox1{
    width: 50%;
  }
  .home_sectionD .home_Dbox1 img{
    width: 100%;
  }
  .home_sectionD .home_Dbox2{
    width: 50%;
  }
  .home_sectionD h1{
    font-size: 50px;
    font-weight: bold;
  }
  .home_sectionD p{
    font-size: 25px;
  }

  /* home footer */

    .home_footer{
    width: 100%;
    padding: 40px 10px;
  }
  .home_Fheader{
    width: 85%;
    margin: 0 auto;
    margin-bottom: 14px;
  }
  .home_Fheader a{
    color: #6F7368;
    text-decoration: none;
  }
  .home_Fheader a:hover{
    color: #6F7368;
    text-decoration: underline;
  }
  .home_Fbox{
    width: 85%;
    display: flex;
    margin: 0 auto;

  }
  .home_Fbox a{
    display: block;
    font-size: 14px;
    margin-top: 8px;
    color: #6F7368;
    text-decoration: none;
  }
    .home_Fbox a:hover{
    color: #6F7368;
    text-decoration: underline;
  }
  .home_Fcol_1, .home_Fcol_2,.home_Fcol_3,.home_Fcol_4{
    width: 25%;
  }
  .home_Ffoot{
    width: 85%;
    margin: 0 auto;
    margin-top: 20px;
  }
  .home_Ffoot a{
    color: #6F7368;
    font-size: 14px;
    text-decoration: none;
  }

</style>
