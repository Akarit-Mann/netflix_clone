<template>
  <div class="home_question container">
    <div class="home_question_header">
        <h1>Frequently Asked Questions</h1>
    </div>
    <div class="question_container">

       <div class="question_box" >
            <div class="question" @click="questionShow1 =! questionShow1">
                <h1>What is Netflix?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow1"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow1">
                <p>Netflix is a streaming service that offers a wide variety of award-winning TV shows, movies, anime, documentaries, and more on thousands of internet-connected devices.</p>
                <p>You can watch as much as you want, whenever you want without a single commercial – all for one low monthly price. There's always something new to discover and new TV shows and movies are added every week!</p>
            </div>
       </div>

       <div class="question_box" >
            <div class="question" @click="questionShow2 =! questionShow2">
                <h1>How much does Netflix cost?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow2"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow2">
                <p>Watch Netflix on your smartphone, tablet, Smart TV, laptop, or streaming device, all for one fixed monthly fee. Plans range from USD3.99 to USD11.99 a month. No extra costs, no contracts.</p>
            </div>
       </div>

       <div class="question_box" >
            <div class="question" @click="questionShow3 =! questionShow3">
                <h1>Where can I watch?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow3"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow3">
                <p>Watch anywhere, anytime. Sign in with your Netflix account to watch instantly on the web at netflix.com from your personal computer or on any internet-connected device that offers the Netflix app, including smart TVs, smartphones, tablets, streaming media players and game consoles.</p>
                <p>You can also download your favorite shows with the iOS, Android, or Windows 10 app. Use downloads to watch while you're on the go and without an internet connection. Take Netflix with you anywhere.</p>
            </div>
       </div>

       <div class="question_box" >
            <div class="question" @click="questionShow4 =! questionShow4">
                <h1>How do I cancel?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow4"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow4">
                <p>Netflix is flexible. There are no pesky contracts and no commitments. You can easily cancel your account online in two clicks. There are no cancellation fees – start or stop your account anytime.</p>
            </div>
       </div>

       <div class="question_box" >
            <div class="question" @click="questionShow5 =! questionShow5">
                <h1>What can I watch on Netflix?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow5"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow5">
                <p>Netflix has an extensive library of feature films, documentaries, TV shows, anime, award-winning Netflix originals, and more. Watch as much as you want, anytime you want.</p>
            </div>
       </div>

       <div class="question_box" >
            <div class="question" @click="questionShow6 =! questionShow6">
                <h1>Is Netflix good for kids?</h1>
                <div class="icon_box">
                    <i class="fa-solid fa-xmark" v-if="questionShow6"></i>
                    <i class="fa-solid fa-plus" v-else></i>
                </div>
            </div>
            <div class="answer" v-if="questionShow6">
                <p>You can watch as much as you want, whenever you want without a single commercial – all for one low monthly price. There's always something new to discover and new TV shows and movies are added every week!</p>
                <p>Kids profiles come with PIN-protected parental controls that let you restrict the maturity rating of content kids can watch and block specific titles you don’t want kids to see.</p>
            </div>
       </div>

    </div>

    <div class="mt-5">
        <p>Ready to watch? Enter your email to create or restart your membership.</p>
        <div class="inputField">
            <input type="email" placeholder="Email address">
            <div>
                Get Started 
                <i class="fa-thin fa-greater-than"></i>
            </div>
        </div>
    </div>


  </div>
</template>

<script>
import { ref } from '@vue/reactivity'
export default {

    setup(props) {
        let questionShow1= ref(false);
        let questionShow2= ref(false);
        let questionShow3= ref(false);
        let questionShow4= ref(false);
        let questionShow5= ref(false);
        let questionShow6= ref(false);
        
        
        return{
            questionShow1,
            questionShow2,
            questionShow3,
            questionShow4,
            questionShow5,
            questionShow6,
        }
    }

}
</script>

<style>


    .inputField{
        display: flex;
        width: 100%;
        max-width: 650px;
        align-items: center;
        margin: 0 auto;
        background-color: red;
    }
    .inputField input{
        width: 70%;
        padding:20px 10px;
    }
    .inputField div{
        width: 30%;
        padding: 10px;
        font-size: 25px;
    }




    .home_question{
        width: 100%;
        padding: 50px 10px;
        display: flex;
        flex-direction: column;
        text-align: center;
    }
    .home_question .home_question_header h1{
        font-size: 50px;
        font-weight: bold;
        margin-bottom: 35px;
    }
    .question_container{
        width: 100%;
        max-width: 850px;
        margin: 0 auto;
    }
    .question_box{
        width: 100%;
        background-color: #303030;
        color: #fff;
        margin-bottom: 10px;
    }
    .question{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 13px 30px;
        border-bottom: 1px solid black;
    }
    .question h1{
        font-size: 30px;
    }
    .question_box .icon_box{
        font-size: 35px;
    }
    .answer{
        text-align: start;
        padding: 15px 30px;
        font-size: 23px;
    }
</style>