<template>
  <section class="contacts">
      <div class="container">
          <div class="row">
              <div class="offset-3 col-6">
                  <h2 class="contacts__title">Contact with our team</h2>
                  <p class="contacts__text">If you are planning on developing a product landing.</p>
              </div>
          </div>

            <div class="row gx-5">
                <div class="col-6">
                    <img src="../../assets/images/StaticMapService.GetMapIma.png" alt="San Francisco Map">
                </div>

                <div class="col-6 contacts__info">
                    <LogoandLogoText/>
                    <p class="contacts__address">9840 Shore St. Fond Du Lac, WI 549335</p>
                    <p class="contacts__phone">0 1223 456 789</p>
                    <p class="contacts__mail">mail@sofbox.com</p>
                    
                    <!-- Social Network icons -->
                    <Socials/> 
                    <!-- / Social Network icons -->

                    <!-- Contact form -->
                    <h4>Get in Touch</h4>
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
                                <textarea name="message" id="message" cols="30" rows="10" class="form-control" placeholder="Your Message"></textarea>
                            </div>
                        </div>

                        <Button>Send Message</Button>

                    </form>
                    <!-- / Contact form -->
                </div>
          </div>
        </div>
  </section>
</template>

<script>
import LogoandLogoText from "../elements/LogoandLogoText.vue";
import Socials from "../elements/Socials.vue";
import Button from "../elements/Button.vue";

export default {
    name: "Contacts",
    components: {
        LogoandLogoText,
        Socials,
        Button
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.contacts {
    text-align: center;
    margin-bottom: 100px;

    &__text {
        margin-bottom: 80px;
    }

    &__info {
        text-align: left;
    } 

    &__address {
        color: $text-primary;
        font-size: 20px;
        font-weight: 500;
    }

    &__phone, 
    &__mail {
        margin: 0;
        color: $text-grey;
        font-size: 14px;
        font-weight: 500;
    }

    textarea {
        padding: 15px;
        margin-bottom: 35px;
    }
}
</style>