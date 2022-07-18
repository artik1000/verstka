<template>
    <div class="selector">
        <div class="selector__item"
             v-for="option in optionsSelect"
             :key="option.id"
             :class="{selector__item__selected: option.selected}"
             @click="selectOption(option)"
        >
            {{option.title}}
        </div>
    </div>
</template>
<script>
export default {
   name: 'my-select',
    props: {
        optionsSelect: {
            type: Array,
            required: true
        },
    },
    methods: {
       selectOption (option) {
           this.$emit('selectReset');
           option.selected = true;
       }
    }
}
</script>
<style lang="sass" scoped>
.selector
    font-style: normal
    font-weight: 500
    font-size: 16px
    line-height: 17px
    letter-spacing: -0.01em
    color: #000000
    display: flex
    flex-direction: row
    align-items: center
    justify-content: center
    .selector__item
        border-bottom: 1px solid rgba(0, 0, 0, 0.33)
        padding: 20px
        text-align: center
    .selector__item__selected
        padding: 20px
        border-bottom: 1px solid #000000
        text-align: center
@media screen and (max-width: 1024px)
    .selector
        margin-top: 24px
        font-style: normal
        font-weight: 500
        font-size: 16px
        line-height: 17px
        letter-spacing: -0.01em
        color: #000000
        display: flex
        flex-direction: row
        .selector__item
            border-bottom: 1px solid rgba(0, 0, 0, 0.33)
            padding: 20px
            width: 100%
            text-align: center
        .selector__item__selected
            text-align: center
            padding: 20px
            border-bottom: 1px solid #000000
            width: 100%
</style>