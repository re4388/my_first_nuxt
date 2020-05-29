<template>
  <img
    class="GithubLogo"
    alt="Github Logo"
    src="/github-logo.png"
  >
</template>

<style>
.GithubLogo {
  height:79px;
  width: 151px;
  transform: rotateY(560deg);
  animation: turn 3.5s ease-out forwards 1s;
}

@keyframes turn {
  100% {
    transform: rotateY(0deg);
  }
}
</style>
