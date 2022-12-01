<template>
    <section class="skills section container" id="skills">
        <h2 class="section__title">Skills</h2>
        <span class="section__subtitle">My technical level</span>

        <div class="skills__container grid">
            <div>
                <div class="skills__content">
                    <div class="skills__header">
                        <div>
                            <i class="uil uil-brackets-curly skills__icon"></i>
                            <h3 class="skills__title">Frontend developer</h3>
                        </div>

                        <i @click.stop ="frontendList = true" v-if="!frontendList" class="uil uil-plus-circle skills__arrow"></i>
                        <i @click.stop ="frontendList = false" v-else class="uil uil-minus-circle skills__arrow-close"></i>
                    </div>

                    <div class="skills__list" v-if="frontendList">
                        <h4>HTML</h4>
                        <h4>CSS | Flexbox | Grid</h4>
                        <h4>SCSS | Bootstrap</h4>
                        <h4>JavaScript</h4>
                        <h4>Vue 3</h4>
                        <h4>Vuex | Vue-router</h4>
                        <h4>GitHub | Git</h4>
                    </div>
                </div>
            </div>
            <div>
                <div class="skills__content">
                    <div class="skills__header">
                        <div>
                            <i class="uil uil-database skills__icon"></i>
                            <h3 class="skills__title">Backend developer</h3>
                        </div>

                        <i v-if="!backendList"  @click.stop ="backendList = true"  class="uil uil-plus-circle skills__arrow"></i>
                        <i v-if="backendList" @click.stop ="backendList = false" class="uil uil-minus-circle skills__arrow-close"></i>
                    </div>

                    <div class="skills__list" v-if="backendList">
                        <h4>Node.js</h4>
                        <h4>Express</h4>
                        <h4>Nodemon</h4>
                        <h4>Webpack</h4>
                        <h4>Postgres</h4>
                    </div>
                </div>
            </div>
            <div>
                <div class="skills__content">
                    <div class="skills__header">
                        <div>
                            <i class="uil uil-palette skills__icon"></i>
                            <h3 class="skills__title">Designer</h3>
                        </div>

                        <i v-if="!designerList"  @click.stop ="designerList = true" class="uil uil-plus-circle skills__arrow"></i>
                        <i v-if="designerList" @click.stop ="designerList = false"  class="uil uil-minus-circle skills__arrow-close"></i>
                    </div>

                    <div class="skills__list" v-if="designerList">
                        <h4>Figma</h4>
                        <h4>Adobe XD</h4>
                        <h4>Sketch</h4>
                        
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            frontendList: true,
            backendList: false,
            designerList: false,
        }   
    },


}
</script>
