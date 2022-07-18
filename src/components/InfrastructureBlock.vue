<template>
<section class="infr__background">
 <h1 class="infr__text">Инфраструктура</h1>
    <my-selector
            :selecte="options"
            :items="selectItems"
    />
</section>
</template>
<script>
import MySelector from "@/components/MySelector/MySelector";
export default {
    name:'infrastructure-block',
    components: {MySelector},
    data () {
        return {
            selectItems: [
                {id: 1, title: 'Газ', url: '/static/Gas.svg'},
                {id: 2, title: 'Электричество', url: '/static/Electro.svg'},
                {id: 3, title: 'Водопровод', url: '/static/Water.svg'},
                {id: 4, title: 'Канализация', url: '/static/Toilet.svg'},
                {id: 5, title: 'Благоустройство', url: '/static/Three.svg'},
                {id: 6, title: 'Интернет', url: '/static/Antenna.svg'},
            ],
            options: [
                {id: 1, title: 'Внутри', selected: true},
                {id: 2, title: 'Рядом', selected: false}
            ]
        }
    },
}
</script>
<style lang="sass" scoped>
.infr__background
    background: url("@/assets/res.png")
    background-repeat: no-repeat
    display: flex
    flex-direction: column
    padding-bottom: 113px
.infr__text
    margin-top: 107px
    margin-left: 107px
    font-style: normal
    font-weight: 400
    font-size: 56px
    line-height: 58px
    letter-spacing: -0.01em
    color: #000000
@media screen and (max-width: 1024px)
    .infr__background
      background: white
      padding-bottom: 40px
    .infr__text
     margin-top: 70px
     margin-left: 24px
     font-style: normal
     font-weight: 400
     font-size: 28px
     line-height: 28px
     letter-spacing: -0.01em
     color: #000000
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