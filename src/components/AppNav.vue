<template>
  <!-- <header>
    <nav>
      <h1>Navigation</h1>
    </nav>
  </header> -->

  <header>
    <div class="hero-container pad">
      <nav class="navbar" id="nav">
        <ul class="right-nav" id="links">
          <li><a class='link' href="">About Us</a></li>
          <li><a class='link' href="">Offers</a></li>
          <li><a class='link' href="">Careers</a></li>
          <li><a class='link' href="">Our Journey</a></li>
          <li><button class="nav-btn">Get In Touch</button></li>
        </ul>
      </nav>
    </div>
  </header>





</template>

<script>
export default {
name:"AppNav",
}
</script>

<style scoped>


header{
    height: 100px;
    background-color: rgb(221, 194, 43);
    display: flex;
    text-align: center;
    /* margin-bottom: 10px;  */
    margin-top: -50px;

}
.hero-container {
  height: 160px;
  padding-left: 60%;
  
  /* padding-right: 10%; */
}
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 15px;
}
.right-nav {
  display: flex;
  list-style: none;
}

.right-nav li {
  margin-left: 0px;
  
}
.link {
  text-decoration: none;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
  text-align: center;
  color: black;
  margin-right: 50px;
}
.nav-btn {
  height: 35px;
  width: 146px;
  background: #ffffff;
  border-radius: 24.1026px;
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  color: black;
    padding: 8px;
    font-size: 16px;
    /* background-color: gold; */
}
</style>