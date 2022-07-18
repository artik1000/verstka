<template>
<section class="gen__plan">
    <h1 class="gen__plan__text">Ген. план </h1>
    <img class="gen__plan__img" src="@/assets/GenPlan.svg">
    <img class="compas" src="@/assets/Compas.svg">
</section>
</template>
<script>
export default {
    name: 'gen-plan'
}
</script>
<style lang="sass" scoped>
.gen__plan
    background: #f0f2f5
.gen__plan__text
    font-style: normal
    font-weight: 400
    font-size: 56px
    line-height: 103.61%
    text-align: right
    letter-spacing: -0.01em
    color: #202020
    position: absolute
    top: 59px
    right: 141px
.gen__plan__text::after
    content: "поселка"
    font-weight: 700
.compas
    position: absolute
    bottom: 64px
    right: 198px
@media screen and (max-width: 1024px)
 .gen__plan
     padding-top: 24px
 .gen__plan__text
    font-style: normal
    font-weight: 400
    font-size: 28px
    line-height: 28px
    text-align: left
    letter-spacing: -0.01em
    color: #202020
    position: static
    margin-top: 23px
    margin-left: 16px
 .gen__plan__text::after
    content: "поселка"
    font-weight: 700
 .compas
    position: absolute
    width: 85px
    height: 89px
    top: 23px
    right: 16px
</style>