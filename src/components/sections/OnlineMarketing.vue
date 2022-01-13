<template>
    <section class="marketing">
        <div class="container">
            <Card v-for="(card, index) in cards" :key="index" :card="card"/>
        </div>
  </section>
</template>

<script>
import Card from "../elements/Card.vue";

export default {
    name: "OnlineMarketing",
    components: {
        Card
    },
    data() {
        return {
            cards: [
                {
                    title: "Online Marketing",
                    subtitle: "It is a long established fact that a reader will be distracted",
                    infos: [
                        "SEO",
                        "SEM",
                        "Website Strategy",
                        "Social management"
                    ]
                },
                {
                    title: "Online Marketing",
                    subtitle: "It is a long established fact that a reader will be distracted",
                    infos: [
                        "SEO",
                        "SEM",
                        "Website Strategy",
                        "Social management"
                    ]
                },
                {
                    title: "Online Marketing",
                    subtitle: "It is a long established fact that a reader will be distracted",
                    infos: [
                        "SEO",
                        "SEM",
                        "Website Strategy",
                        "Social management"
                    ]
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.marketing {
    margin-top: 150px;

    .container {
        display: flex;
    }
}
</style>