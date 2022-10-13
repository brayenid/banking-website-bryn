<template>
  <div class="hamburger flex sm:hidden">
    <input class="hamCheck" type="checkbox" name="" id="" />
    <span></span>
    <span></span>
    <span></span>
  </div>
</template>
<style scoped>
.hamburger {
  width: 35px;
  height: 28px;
  position: relative;
  flex-direction: column;
  justify-content: space-around;
}
.hamburger input {
  position: absolute;
  width: 100%;
  height: 100%;
  margin-top: -1px;
  margin-left: -1px;
  opacity: 0;
  z-index: 10;
  cursor: pointer;
}
.hamburger span {
  width: 100%;
  height: 4px;
  border-radius: 10px;
  background-color: black;
  transition: 0.3s cubic-bezier(0.17, 0.67, 0.83, 0.67);
}
.hamburger input:checked ~ span:nth-child(2) {
  transform: rotate(20deg);
  width: 80%;
}
.hamburger input:checked ~ span:nth-child(3) {
  transform: rotate(20deg);
  width: 90%;
}
.hamburger input:checked ~ span:nth-child(4) {
  transform: rotate(20deg);
  width: 100%;
}
</style>
