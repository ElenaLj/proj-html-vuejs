<template>
    <div class="cards">
        <div class="row">
            <div class="col-3">
                <img src="../../assets/images/24.png" alt="Television icon" class="cards__img">
            </div>

            <div class="col-9">
                <h5>{{card.title}}</h5>
                <p class="cards__text">{{card.subtitle}}</p>
                <ul class="cards__list">
                    <li v-for="(info, index) in card.infos" :key="index" class="cards__item">
                        <i class="fas fa-check cards__icon"></i>
                        <span>{{info}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Card",
    props: {
        card: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.cards {
    width: calc(100% / 3);
    
    &__img {
        height: 80px;
    }

    &__text {
        color: $text-grey;
    }

    &__list {
        list-style: none;
        padding-left: 0;
    }

    &__item {
        padding: 10px 0;
        font-weight: 500;
    }

    &__icon {
        margin-right: 15px;
        color: $text-blue;
    }
}
</style>