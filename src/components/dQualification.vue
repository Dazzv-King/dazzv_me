<template>
    <section class="qualification section" id="qualification">
        <h2 class="section__title">Qualification</h2>
        <span class="section__subtitle">My personal journey</span>

        <div class="qualification__container container">
            <div class="qualification__tabs">
                <div @click="educationList = true" class="qualification__button button--flex" :class="{qualification__button__active: educationList}">
                    <i class="uil uil-graduation-cap qualification__icon"></i> Education
                </div>
                <div @click="educationList = false" class="qualification__button button--flex" :class="{qualification__button__active: !educationList}">
                    <i class="uil uil-briefcase-alt qualification__icon"></i> Work
                </div>
            </div>

            <div class="qualification__sections">
                <div v-if="educationList" class="qualification__content">
                    <div class="qualification__data">
                        <div>
                            <h3 class="qualification__title">Computer Engineer</h3>
                            <span class="qualification__subtitle">Samara - University</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                2019 - 2023
                            </div>
                        </div>

                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>

                        <div></div>
                    </div>
                    <div class="qualification__data">
                        <div></div>
                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>
                       
                        <div>
                            <h3 class="qualification__title">Learning how to Learn</h3>
                            <span class="qualification__subtitle">Coursera</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                05.2022 - 09.2022
                            </div>
                        </div>
                    </div>
                    <div class="qualification__data">
                        <div>
                            <h3 class="qualification__title">Vue 3</h3>
                            <span class="qualification__subtitle">JavaScript.ninja</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                04.2022 - 08.2022
                            </div>
                        </div>

                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>
                        <div></div>
                    </div>
                    <div class="qualification__data">
                        <div></div>
                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>

                        <div>
                            <h3 class="qualification__title">Vue.js</h3>
                            <span class="qualification__subtitle">Metanit</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                11.2021 - 01.2022
                            </div>
                        </div>
                    </div>
                    <div class="qualification__data">
                        <div>
                            <h3 class="qualification__title">JavaScript</h3>
                            <span class="qualification__subtitle">Code Basics</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                10.2021 - 12.2021
                            </div>
                        </div>

                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>
                        <div></div>
                    </div>
                    <div class="qualification__data">
                        <div></div>
                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>

                        <div>
                            <h3 class="qualification__title">Web. Frontend</h3>
                            <span class="qualification__subtitle">Stepik</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                07.2021 - 09.2021
                            </div>
                        </div>
                    </div>
                    <div class="qualification__data">
                        <div>
                            <h3 class="qualification__title">Intro to Web</h3>
                            <span class="qualification__subtitle">HTML Academy</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                09.2020 - 12.2020
                            </div>
                        </div>
                        
                        <div>
                            <span class="qualification__rounder"></span>
                            <!-- <span class="qualification__line"></span> -->
                        </div>
                        <div></div>
                    </div>
                </div>
                <div v-else class="qualification__content">
                    <div class="qualification__data">
                        <div>
                            <h3 class="qualification__title">Trainee | JS dev</h3>
                            <span class="qualification__subtitle">Mediasoft - Samara</span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                06.2022 - 08.2022
                            </div>
                        </div>
                        <div>
                            <span class="qualification__rounder"></span>
                            <span class="qualification__line"></span>
                        </div>
                        <div></div>
                    </div>
                    <div class="qualification__data">
                        <div></div>
                        <div>
                            <span class="qualification__rounder"></span>
                            <!-- <span class="qualification__line"></span> -->
                        </div>
                        <div>
                            <h3 class="qualification__title">Frontend developer</h3>
                            <span class="qualification__subtitle">Freelance | University </span>
                            <div class="qualification__calendar">
                                <i class="uil uil-calendar-alt"></i>
                                06.2021 - 05.2022
                            </div>
                        </div>
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
            educationList: true,
        }
    },
}
</script>
