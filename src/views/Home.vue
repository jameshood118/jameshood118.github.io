<template>
  <div class="columns">
    <div class="column">
      <div class="card" v-for="items in home" :key="items.title">
        <header class="card-header">
          <p class="card-header-title">
            {{items.title}} </p>
        </header>
        <div class="card-content">
          <div class="content" v-html="items.message">

            <br>
            <time :datetime="items.date">{{items.date}}</time>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return{
home: [
  {title: "Welcome to my Portfolio", date:"6/03/2018", message: "Welcome to my portfolio, This website is to represent myself to the corporate world, and as such this site contains my artwork, and my web development work. It also happens to contain various side projects: Music, various video/audio projects I will work on from time to time, and other side projects. I also use this site as a means to test out code that I am working on, or have been tasked to do. </p><p>I am an outside the box kind of thinker. I am not set in my ways, nor have I had 'the rules of the internet' engraved in my head. If something doesn't work, I find another solution, learn it, and apply it. My methods have always been 'work on it until it works without issues'. I love getting down deep into code and figuring out the logic.</p>"}
]
    }
  }
}
</script>

<style>
</style>
