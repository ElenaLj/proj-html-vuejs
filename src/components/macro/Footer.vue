<template>
  <footer class="footer">
    <div class="container">
      <div class="row">

        <div class="col-3">
          <!-- <img src="../../assets/images/35.png" alt="Sofbox Logo" class="footer__logo"> -->
          <LogoandLogoText/>
          <p class="footer__text">It is a long established fact that a reader will be distracted by the readable content</p>
          <p class="footer__text">Copyright <em>@</em> 2018 <span class="footer__blue">Sofbox</span></p>
        </div>

        <div class="offset-1 col-2">
          <FooterLinks :items="items"/>
        </div>

        <div class="col-3">
          <FooterElms :elm="elm"/>
        </div>

        <div class="col-3">
          <FooterActions :actions="actions"/>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import LogoandLogoText from "../elements/LogoandLogoText.vue";
import FooterLinks from "../elements/FooterLinks.vue";
import FooterElms from "../elements/FooterElms.vue";
import FooterActions from "../elements/FooterActions.vue";

export default {
    name: "Footer",
    components: {
      LogoandLogoText,
      FooterLinks,
      FooterElms,
      FooterActions
    },
    data() {
      return {
        items: [
          {
            text: "About Us",
            url: "#",
            current: false
          },
          {
            text: "Theme",
            url: "#",
            current: false
          },
          {
            text: "Features",
            url: "#",
            current: false
          },
          {
            text: "Pricing",
            url: "#",
            current: false
          },
          {
            text: "Blog",
            url: "#",
            current: false
          }
        ],
        elm: [
          {
            text: "About Sofbox",
            url: "#",
            current: false
          },
          {
            text: "Roadmap",
            url: "#",
            current: false
          },
          {
            text: "How It Works",
            url: "#",
            current: false
          },
          {
            text: "Team",
            url: "#",
            current: false
          },
          {
            text: "News",
            url: "#",
            current: false
          }
        ],
        actions: [
          {
            text: "About Us",
            url: "#",
            current: false
          },
          {
            text: "Theme",
            url: "#",
            current: false
          },
          {
            text: "Features",
            url: "#",
            current: false
          },
          {
            text: "Pricing",
            url: "#",
            current: false
          },
          {
            text: "Blog",
            url: "#",
            current: false
          }
        ]  
      }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.footer {
  font-weight: 500;
  padding: 80px 0;
  border-top: 1px solid $border-grayscale-three;
  
  &__logo {
    height: 3.75rem;
  }

  &__text {
    color: $text-grey;
    margin-top: 30px;

    .footer__blue {
      color: $text-blue;
    }
  }
}
</style>