<template>
  <AppNav />
  <div class="container">
    <img class="background-img" alt="Spa logo" src="./assets/1.jpg"> 
    <h1 class="heading">{{headtitle}}</h1>
    <p class="subheading">{{paragraph}}</p>
    <!-- <h1> {{title}} </h1> -->
    <!-- <p> {{text}} </p> -->
    <!-- <h1>{{fullName}}</h1> -->
    <!-- <h2>{{count}}</h2>
  <button @click="increment">increment</button>
  <button @click="decrement">decrement</button> -->
    <!-- <ul>
      <li v-for="bird in birds" :key="bird">
        {{bird}}
      </li>
    </ul> -->
    <AppButton id="button-one" text="Click for more info" />
    <div class="card-container">
      <AppCard v-for="card in cardData" :key="card.id" :cardImage="card.image" :cardText="card.text"
        :cardHeading="card.heading" />
    </div>
    <br>
    <br>
    <br>
    <br>
    <AppButton id="button-two" text="Choose a Package!" />
  </div>

  <Footer />
</template>

<script>
import Footer from "./components/Footer.vue"
import AppCard from "./components/AppCard.vue"
import AppNav from  "./components/AppNav.vue"
import AppButton from "./components/AppButton.vue"
export default {
  name: 'App',
  components:{AppButton,AppNav,AppCard,Footer},
  data() {
    return {
      cardData: [
        {
          id: "testOne",
          heading: "Premium Package",
          text: "Double occupancy stay in our private cabin. All cabins have private pools and amply manicured lawn areas for private functions. Personalized butler service throughout your stay. Eco-friendly electric carts transportation service. Unlimited supply of soft drinks and hard liquor (In-room only). Unlimited supply of natural and processed snacks. Access to onsite medical professional",
          image:require('@/assets/Package1.jpeg'),
        },
        {
          id: "testTwo",
          heading: "Gold Package",
          text: "These spacious cabins boasts of amazing panoramic views of the valley, the safari and other neighbouring land reserves. Each of these cabins has a balcony and all come with king-size beds and en-suite bathrooms. Suitable for partners and really, any two people. Right outside, you’ll find a complete private outdoor hot tub and sundeck.",
           image: require('@/assets/Package 2.jpeg'),
        },
        {
          id: "testThree",
          heading: "Silver Package",
          text: "Stay in our private cabin for up to four (4) occupants. Connecting cabins have private pool and amply manicured lawn areas for private functions. Personalized butler service throughout your stay. Eco-friendly electric carts transportation service. Unlimited supply of soft drinks and hard liquor (In-room only). Unlimited supply of natural and processed snacks. Access to onsite medical professional.",
          image: require('@/assets/package 3.jpeg'),
        },
        {
          id: "testFour",
          heading: "Platinum package",
          text: "Our Exclusive vacation homes are larger residences that can accommodate the entire family. With an impressive bar, space for game tables and an enormous 26-foot sofa, the vacation home is the place for relaxed and family/group fun times.",
          image: require('@/assets/package 4.jpeg'),
        },
      ],
      paragraph: "Welcome to the KpaKpaKpa resort and spa, your home away from home where you can relax and will be treated like royalty. Come and enjoy our world class accommodation and recreational facilities that provide world class services to its guests.  Ultimately, this brand seeks to replicate God’s handiwork in the biblical Garden of Eden, here in the serene natural habitat that KpaKpaKpa offers. ",
      headtitle:"Home Away from Home"
      // title: "Learning Vue",
      // text: "This is working",
      // count: 0,
      // firstName: "Calvin",
      // lastName: "Mends",
      // birds:["Doves","Eagles","Hawks","Pigeons"],
    };
  },
  methods: {
    // increment() {
    //   this.count++;
    // },
    // decrement() {
    //   this.count--;
    // },
  },
  computed: {
    // fullName() {
    //   return`${this.firstName} ${this.lastName}`
    // }
  }
}
</script>

<style>
*{
padding: 0;
margin: 0;
box-sizing: border-box;

}
.container{
  /* max-width: 60%; */
  margin: 0 auto;
  text-align: center;
  align-items: center;
}
/* img{
  width: 300px;
  height: 100px;
} */

.heading {
  font-style: normal;
  font-weight: 700;
  font-size: 53.7049px;
  line-height: 73px;
  color: rgb(228, 164, 81);
  margin-top: 50px;
}
.subheading {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 35px;
  color: black;
  margin-top: 21px;
}
#button-one {
  margin-top: 30px;
  border-radius: 30px;
}
#button-two{
  margin-top:30px ;
  border-radius: 30px;
}
.card-container {
  display: flex;
  /* flex-direction: column; */
  gap: 5px;
  align-items: center;
  width: 100%;
  text-align: center;
  margin-bottom: 80px;
  margin-top: 40px;
}
.background-img{
  width: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 50px;
}
</style>


