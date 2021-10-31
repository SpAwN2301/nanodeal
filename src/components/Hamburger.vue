<template>
  <div @click="showNavPanel" class="hamburger"><span></span><span></span><span></span></div>
</template>

<script>
export default {
  name: "Hamburger",
  
  methods: {
    showNavPanel () {
      const hamburger = document.querySelector('.hamburger');
      const navPanel = document.querySelector('.nanodeal__nav')

      hamburger.classList.toggle('active')
      navPanel.classList.toggle('active')
    }
  }
};
</script>

<style>
.hamburger {
  display: none;
}
.hamburger span {
  display: block;
  margin: 2px 0;
  height: 2px;
  width: 100%;
  background-color: #2d3134;
  transition: 0.5s;
}
.hamburger span:nth-child(1) {
  width: 20px;
}
.hamburger span:nth-child(2) {
  width: 10px;
}
.hamburger span:nth-child(3) {
  width: 15px;
}

.hamburger.active span:nth-child(1) {
  transform: translateY(4px) rotate(-45deg);
}
.hamburger.active span:nth-child(2) {
  display: none;
}
.hamburger.active span:nth-child(3) {
  transform: rotate(45deg);
  width: 20px;
}

@media screen and (max-width: 768px) {
  .hamburger {
    cursor: pointer;
    position: relative;
    z-index: 3;
    display: block;
  }
}
</style>
