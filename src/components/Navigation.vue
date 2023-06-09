<script setup lang="ts">
import { RouterLink } from 'vue-router';
</script>


<template>
    <nav>
      <input type="checkbox" id="check">
      <label for="check" class="checkbtn">
        <i class="fas fa-bars"></i>
      </label>
      <label class="logo">
        <RouterLink to="/">
            <img alt="Vue logo" class="logo" src="@/assets/logo.svg"  />
        </RouterLink>
      </label>
      <ul>
        <li>
            <RouterLink to="/about" class="gradient-text">Services</RouterLink>
        </li>
        <li>
            <RouterLink to="/about" class="gradient-text">Works</RouterLink>
        </li>
        <li>
            <RouterLink to="/about" class="gradient-text">About</RouterLink>
        </li>
        <li>
            <RouterLink to="/about" class="gradient-text">Clients</RouterLink>
        </li>
        <li>
            <RouterLink to="/about" class="gradient-text">Career</RouterLink>
        </li>
        <li>
            <RouterLink to="/about" class="contact-router gradient-back">Contact</RouterLink>
        </li>
      </ul>
    </nav>
</template>
<style lang="scss">

   nav{
  background: none;
  height: 100px;
  width: 100%;
  position: fixed;
  z-index: 1000;
  backdrop-filter: blur(20px);
  top: 0;
  background: rgba(19, 19, 19, 0.8674466);
  padding: 10px 4%;
}
label.logo{
  color: white;
  font-size: 35px;
  line-height: 80px;
  font-weight: bold;

  img {
    width: 87px;
    height: 80px;
  }
}
nav ul{
  float: right;
  margin-right: 20px;
}
nav ul li{
  display: inline-block;
  line-height: 80px;
  margin: 0 5px;
}
nav ul li a{
  color: white;
  font-size: 18px;
  padding: 7px 10px;
  margin: 0 5px;
  border-radius: 3px;
  border: 2px solid rgba(0, 0, 0, 0);
  font-family: 'Bagel Fat One', cursive;
  transition: .3s ease-out;
  text-transform: uppercase;

  &:hover {
    filter: drop-shadow(0 0 0.65rem var(--var-color-prim));
  }

}
.checkbtn{
  font-size: 30px;
  color: white;
  float: right;
  line-height: 80px;
  margin-right: 40px;
  cursor: pointer;
  display: none;
}
#check{
  display: none;
}
@media (max-width: 952px){
  label.logo{
    font-size: 30px;
    padding-left: 50px;
  }
  nav ul li a{
    font-size: 16px;
  }
}
@media (max-width: 858px){
  .checkbtn{
    display: block;
  }
  ul{
    position: fixed;
    width: 100%;
    height: 100vh;
    background: #2c3e50;
    top: 80px;
    left: -100%;
    text-align: center;
    transition: all .5s;
  }
  nav ul li{
    display: block;
    margin: 50px 0;
    line-height: 30px;
  }
  nav ul li a{
    font-size: 20px;
  }
  a:hover,a.active{
    background: none;
    color: #0082e6;
  }
  #check:checked ~ ul{
    left: 0;
  }
}
section{
  background: url(bg1.jpg) no-repeat;
  background-size: cover;
  height: calc(100vh - 80px);
}
.contact-router {
    border: none;
    color: var(--var-color-white);
    margin: 7px 10px;
    padding: 14px 20px;
    text-decoration: none;

    &:hover {
        border: none;
        filter: brightness(1.2);
    }
}
</style>