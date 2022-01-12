<template>
  <section class="contacts">
      <div class="container">
          <div class="row">
              <div class="offset-3 col-6">
                  <h2 class="contacts__title">Contact with our team</h2>
                  <p class="contacts__text">If you are planning on developing a product landing.</p>
              </div>
          </div>

            <div class="row">
                <div class="col-6">
                    <img src="../../assets/images/StaticMapService.GetMapIma.png" alt="San Francisco Map">
                </div>

                <div class="col-6 contacts__info">
                    <LogoandLogoText/>
                    <p class="contacts__address">9840 Shore St. Fond Du Lac, WI 549335</p>
                    <p class="contacts__phone">0 1223 456 789</p>
                    <p class="contacts__mail">mail@sofbox.com</p>
                    
                    <div class="contacts__icons"></div>

                    <!-- Contact form -->
                    <form>
                        <div class="row d-flex g-2">
                            <div class="col-6">
                                <label for="name"></label>
                                <input type="text" class="form-control" id="name" placeholder="Your Name">
                            </div>
                            <div class="col-6">
                                <label for="email"></label>
                                <input type="email" class="form-control" id="email" placeholder="Your Email">
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-12">
                                <label for="subject"></label>
                                <input type="text" class="form-control" id="subject" placeholder="Your Subject">
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-12">
                                <label for="message"></label>
                                <input type="text" class="form-control" id="message" placeholder="Your Message">
                            </div>
                        </div>
                    </form>
                    <!-- / Contact form -->
                </div>
          </div>
        </div>
  </section>
</template>

<script>
import LogoandLogoText from "../elements/LogoandLogoText.vue";

export default {
    name: "Contacts",
    components: {
        LogoandLogoText
    }
}
</script>

<style lang="scss" scoped>
.contacts {
    text-align: center;

    &__info {
        text-align: left;
    } 
}
</style>