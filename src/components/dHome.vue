<template>
  <section class="home section" id="home">
      <div class="home__container container grid">
         <div class="home__content grid">
            <!-- <hr> -->
            <div class="home__social">
               <a href="https://vk.com/dazzv_me" class="home__social-icon" target="_blank">
                  <i class="uil uil-vk-alt"></i>
               </a>
               <a href="https://github.com/Dazzv-King" class="home__social-icon" target="_blank">
                  <i class="uil uil-github-alt"></i>
               </a>
               <a href="https://t.me/dazzv_me" class="home__social-icon" target="_blank">
                  <i class="uil uil-telegram-alt"></i>
               </a>
               <a href="https://career.habr.com/dazzv_me" class="home__social-icon" target="_blank">
                  <i class="uil uil-brain"></i>
               </a>
            </div>
            
            <div class="home__img">
               <img src="../assets/img/me.png" alt="img" class="home__blob-img">
            </div>

            <div class="home__data">
               <h1 class="home__title">Hi, I am Davlat</h1>
               <h3 class="home__subtitle">Frontend developer</h3>
               <p class="home__description">Web developer who focused on creating functional and beautiful websites</p>
               <a href="#contact" class="button button--flex">
                  Contact Me<i class="uil uil-message button__icon"></i>
               </a>
            </div>
         </div>
         <div class="home__scroll">
            <a href="#about" class="home__scroll-button button--flex">
               <i class="uil uil-mouse-alt home__scroll-mouse"></i>
               <span class="home__scroll-name">Scroll down</span>
               <i class="uil uil-arrow-down home__scroll-arrow "></i>
            </a>
         </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'HelloWorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

