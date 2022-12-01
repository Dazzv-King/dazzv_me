<template>
    <section class="contact section sec_contact" id="contact">
        <h2 class="section__title">Let<span class="section__title-span">'</span>s Talk</h2>
        <div class="contact__container container">
            <div class="sec_body">
                <div class="contacts sec__body__div">
                    <div class="my">
                    <i class="uil uil-phone-alt contact__icon"></i>
                    <a href="tel:+7 996 624-93-44" type="phone">+7 9966249344</a>
                    </div>
                    <div class="my">
                    <i class="uil uil-envelope-alt contact__icon"></i>
                    <a  href= "mailto: davlat.azizov.4712@gmail.com">davlat.azizov.4712@gmail.com</a>
                    </div>
                    <div class="my">
                    <i class="uil uil-location-point contact__icon"></i>
                    <a href="https://www.google.com/maps/place/Samara">Russia, Samara</a>
                    </div>
                </div>
                <div class="contacts mob__sec__body__div">
                    <div class="my">
                    <a href="tel:+7 996 624-93-44" type="phone"><i class="uil uil-phone-alt contact__icon"></i></a>
                    </div>
                    <div class="my">
                    <a  href= "mailto: davlat.azizov.4712@gmail.com"><i class="uil uil-envelope-alt contact__icon"></i></a>
                    </div>
                    <div class="my">
                     <a href="https://www.google.com/maps/place/Samara"><i class="uil uil-location-point contact__icon"></i></a>
                    </div>
                </div>
                <hr class="contact_secline"/>
                <div class="contactme sec__body__div">
                    <form action="https://formsubmit.co/davlat.azizov.4712@gmail.com" method="POST">
                      <div>
                          <p class="form__title">Ваше имя</p>
                          <input class="form__input" v-model="name" type="text" name="name" placeholder="Имя"/>
                      </div>

                      <div>
                          <p class="form__title">Ваша почта</p>
                          <input class="form__input" v-model="email" type="email" name="email" placeholder="Ваша почта" />
                      </div>

                      <div>
                          <p class="form__title">Сообщение</p>
                          <textarea class="form__textarea" v-model="message" name="message" type="message" placeholder="Сообщение"></textarea>
                      </div>
                      <div class="sec_btn">
                          <a class = "button button--flex" type="submit">Отправить</a>
                          <a @click="onReset" class = "button button--flex" type="reset">Очистить</a>
                      </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
name: "Contact",
  props: true,
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    onReset() {
      this.name = "";
      this.email = "";
      this.message = "";
    },

  },

}
</script>
<style>
    
</style>