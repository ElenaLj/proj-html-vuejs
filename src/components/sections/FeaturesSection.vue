<template>
    <section class="features">
        <div class="container">
            <div class="row features__info">
                <div class="col-8">
                    <h2 class="features__title">Popular features that your business needs</h2>
                    <p class="features__text">Faff about only quid blower I don't want no agro bleeding chimney <br> pot burke tosser cras nice one boot fanny!</p>
                </div>
                <div class="col-3">
                    <Button>Explore More Feature</Button>
                </div>
            </div>
            <div class="features__badges">
                <Badge v-for="(badge, index) in badges" :key="index" :badge="badge"/>
            </div>
        </div>
    </section>
</template>

<script>
import Button from "../elements/Button.vue";
import Badge from "../elements/Badge.vue";

export default {
    name: "FeaturesSection",
    components: {
        Button,
        Badge
    },
    data() {
        return {
            badges: [
                {
                    title: "Customized Invoices",
                    src: require("../../assets/images/001.png"),
                    alt: "Graphic art sketch"
                },
                {
                    title: "Stock Management",
                    src: require("../../assets/images/002.png"),
                    alt: "Graphic art sketch"
                },
                {
                    title: "Receivable & Payables",
                    src: require("../../assets/images/003.png"),
                    alt: "Graphic art sketch"
                },
                {
                    title: "Manage Buying",
                    src: require("../../assets/images/004.png"),
                    alt: "Graphic art sketch" 
                },
                {
                    title: "Powerful & Secure",
                    src: require("../../assets/images/005.png"),
                    alt: "Graphic art sketch"
                },
                {
                    title: "Fastest Return Filing",
                    src: require("../../assets/images/006.png"),
                    alt: "Graphic art sketch" 
                },
                {
                    title: "Monthly Detailed",
                    src: require("../../assets/images/007.png"),
                    alt: "Graphic art sketch"
                },
                {
                    title: "Product Management",
                    src: require("../../assets/images/008.png"),
                    alt: "Graphic art sketch"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.features {
    margin: 100px 0;

    &__info {
        justify-content: space-between;
    }

    &__title {
        margin-bottom: 25px;
    }

    &__badges {
        margin: 30px 0;
    }
}
</style>