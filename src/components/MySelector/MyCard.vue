<template>
    <div class="selector__card">
        <img class="card__icon" :src="item.url">
        <div class="card__title"><p>{{item.title}}</p></div>
    </div>
</template>
<script>
export default {
   name: 'my-card',
   props: {
       item: {
           type: Object,
           required: true
       }
   }
}
</script>
<style lang="sass" scoped>
.selector__card
    background: #FFFFFF
    box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.11)
    border-radius: 12px
    padding-top: 34px
    display: flex
    flex-direction: column
    align-items: center
    justify-content: center
    .card__title
        margin: 30px 68px 33px 68px
        font-style: normal
        font-weight: 400
        font-size: 14px
        line-height: 15px
        letter-spacing: -0.01em
        color: #000000
</style>