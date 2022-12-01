<template>
    <header class="header" id="header">
        <nav class="nav container">
            <div class="nav__log">
                <img class="nav__logo__img" src="../assets/img/dog.gif" type='gif' alt="logo">
                <a href="#" class="nav__logo">Dazzv<span>'</span>s</a>
            </div>

            <div class="nav__menu" id="nav__menu" :class="{'show-menu': isActive}">
                <ul class="nav__list grid">
                    <li class="nav__item">
                        <a href="#home" class="nav__link" @click="isActive = false">
                            <i class="uil uil-estate nav__icon"></i> Home
                        </a>
                    </li>
                    <li class="nav__item">
                        <a href="#about" class="nav__link" @click="isActive = false">
                            <i class="uil uil-user-circle nav__icon"></i> About Me
                        </a>
                    </li>
                    <li class="nav__item">
                        <a href="#skills" class="nav__link" @click="isActive = false">
                            <i class="uil uil-file-alt nav__icon"></i> Skills
                        </a>
                    </li>
                    <li class="nav__item">
                        <a href="#qualification" class="nav__link" @click="isActive = false">
                            <i class="uil uil-graduation-cap nav__icon"></i> Qualification
                        </a>
                    </li>
                    <!-- <li class="nav__item">
                        <a href="#service" class="nav__link">
                            <i class="uil uil-bag-alt .nav__icon"></i> Service
                        </a>
                    </li> -->
                    <li class="nav__item">
                        <a href="#portfolio" class="nav__link" @click="isActive = false">
                            <i class="uil uil-scenery nav__icon"></i> Portfolio
                        </a>
                    </li>
                    <li class="nav__item">
                        <a href="#contact" class="nav__link" @click="isActive = false">
                            <i class="uil uil-message nav__icon"></i> Contacts
                        </a>
                    </li>
                </ul>
                <i @click="isActive = false" class="uil uil-times nav__close" id="nav-close"></i>
            </div>

            <div class="nav__btns">
                <i @click="changeToDarkMode()" class="uil uil-moon change-theme" ref="theme-button" id="theme-button"></i>
                <div @click="show" class="nav__toggle" id="nav-toggle">
                    <i class="uil uil-apps"></i>
                </div>
            </div>
        </nav>
    </header>
</template>
<script>

export default {
    name: "dHeader", 
    data() {
        return {
            isActive: false,
            darkMode: false
        }
    },

    methods: {
        show() {
            this.isActive = true
        },
        changeToDarkMode() {
            this.darkMode = true
            document.body.classList.add('dark-theme')
            
        }
    },
}
</script>


