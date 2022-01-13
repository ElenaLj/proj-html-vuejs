<template>
    <section class="support">
        <div class="container">
            <div class="row">
                <div class="col-6 support__info">
                    <h2 class="support__title">Get tips tricks on how to skyrocket your sales.</h2>
                    <p class="support__text">Faff about only quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny!</p>
                    <Label v-for="(label, index) in labels" :key="index" :label="label"/>
                </div>
                <div class="col-6">
                    <img src="../../assets/images/509.jpeg" alt="Graphic art of people working">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Label from "../elements/Label.vue";

export default {
    name: "TechSupport",
    components: {
        Label
    },
    data() {
        return {
            labels: [
                {
                    img: require("../../assets/images/510.png"),
                    title: "Reporting Analysis",
                    text: "It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout."
                },
                {
                    img: require("../../assets/images/511.png"),
                    title: "Technical SEO Audit",
                    text: "It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.support {
    margin: 150px 0;

    &__info {
        display: flex;
        flex-direction: column;
        gap: 20px;
    }
}
</style>