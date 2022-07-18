<template>
<div class="driving__wrapper">
    <article class="driving__description">
     <h1 class="driving__description__header">Схема </h1>
     <div>
         <p class="driving__text">
             Коттеджный поселок класса De Luxe «Усадьба Бергов» располагается вблизи поселка Первомайское.<br>
             <br>
             Границами участка застройки служат: с севера — улица Парковая, с юга — река Десна и коттеджный поселок «Кедровое», с запада — ИЖС, с востока — ручей.<br>
             <br>
             Подъездная дорога ведет со стороны улицы Парковая поселка Первомайское с выездом на автотрассу «Москва- Киев».
         </p>
     </div>
        <div>
            <div><p class="km">23<br></p></div>
        </div>
    </article>
    <div>
       <img width="100%" src="@/assets/DrivingDirections.svg">
    </div>
</div>
</template>
<script>
export default {
    name: 'driving-directions'
}
</script>
<style lang="sass" scopde>
.driving__wrapper
    display: grid
    grid-template-columns: 50vw 50vw
.driving__description
    display: flex
    flex-direction: column
    gap: 39px
    padding: 38px 115px 38px 115px
.driving__text
    font-style: normal
    font-weight: 500
    font-size: 16px
    line-height: 24px
    letter-spacing: -0.01em
    color: #202020
.driving__description__header
    font-style: normal
    font-weight: 400
    font-size: 56px
    line-height: 58px
    letter-spacing: -0.01em
    color: #202020
.driving__description__header::after
    content: "проезда"
    font-weight: 700
.km
    margin-top: 60px
    font-weight: bold
    font-size: 181px
    color: #6BC067
    text-align: center
    line-height: 40px
.km::after
    content: "км от москвы"
    font-weight: 700
    font-size: 18px
    line-height: 22px
    letter-spacing: -0.01em
    color: #202020
    text-align: center
    margin: 0
@media screen and (max-width: 1024px)
    .driving__wrapper
      display: flex
      flex-direction: column
    .driving__description
     display: flex
     flex-direction: column
     gap: 24px
     padding: 24px 16px 24px 16px
    .driving__description__header
     font-size: 28px
     line-height: 28px
</style>