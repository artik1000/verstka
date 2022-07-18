<template>
    <div class="select__group">
        <my-select
                :optionsSelect="selects"
                @selectReset="removeSelect"
        />
        <div class="selector__cards">
            <my-card
                    v-for="item in items"
                    :key="item.id"
                    :item="item"
                    style="width: 152px"
            />
        </div>
    </div>
</template>
<script>
import MySelect from "./MySelect";
import MyCard from "./MyCard";
export default {
    name: 'my-selector',
    components: {MyCard, MySelect},
    props: {
        items: {
            type: Array,
            required: true
        },
        selecte: {
            type: Array,
            required: true
        },
    },
    data () {
        return {
            selects: []
        }
    },
    methods: {
        removeSelect () {
            for (let i = 0; i < this.selects.length; i++) {
                this.selects[i].selected = false
            }
        }
    },
    beforeMount () {
        this.selects = this.selecte
    }
}
</script>
<style lang="sass" scoped>
.selector__group
    display: flex
    flex-direction: column
    align-items: center
    justify-content: center
.selector__cards
    display: flex
    flex-direction: row
    align-items: center
    justify-content: center
    margin-top: 76px
    gap: 24px
@media screen and (max-width: 1024px)
 .selector__cards
    display: flex
    flex-flow: row
    flex-wrap: wrap
    align-items: center
    justify-content: center
    margin-top: 24px
    gap: 16px
</style>