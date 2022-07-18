<template>
 <section class="about__village__section">
     <div class="about__village__top">
  <article class="about__village__article">
      <div class="about__village__article__header__items">
          <h1 class="about__village__article__header">О поселке</h1>
          <div class="strelka2">
              <svg width="72" height="10" viewBox="0 0 72 10" fill="none" xmlns="http://www.w3.org/2000/svg">
               <path d="M68.3003 5.27782L-1.54751e-05 5.27782L-1.54238e-05 4.10449L68.3003 4.1045L63.4409 1.15676L64.8091 0.329101L72 4.69102L64.8091 9.05212L63.4409 8.22337L68.3003 5.27782Z" fill="#6ED669"/>
              </svg>
          </div>
      </div>
      <div class="about__village__article__text">
          <p>
              Основными элементами планировки участков стали<br>
              уникальные природные условия, ландшафт территории,<br>
              используемой под застройку. Основополагающий фактор<br>
              застройки северной части, на которой расположен лесной<br>
              массив, — сохранение максимального количества вековых<br>
              деревьев. В застройке и планировке участков средней<br>
              части активно используется и сохраняется природный<br>
              ландшафт и рельеф, что позволяет добиться<br>
              уникальных видовых характеристик. В южной части участки<br>
              примыкают к реке, вдоль которой устраивается набережная.<br>
          </p>
      </div>
      <div class="about__village__article__text__mobile">
          <p>
              Основными элементами планировки участков
              стали уникальные природные условия,
              ландшафт территории, используемой под
              застройку. Основополагающий фактор
              застройки северной части, на которой
              расположен лесной массив, — сохранение
              максимального количества вековых деревьев.
              В застройке и планировке участков средней
              части активно используется и сохраняется
              природный ландшафт и рельеф, что позволяет
              добиться уникальных видовых характеристик.
              В южной части участки примыкают к реке,
              вдоль которой устраивается набережная.
          </p>
      </div>
      <div class="about__village__article__more">
          <div>
              <p>Больше о поселке</p>
          </div>
          <div class="strelka">
              <svg width="50" height="14" viewBox="0 0 50 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M46.5532 7.94244L2.26516e-05 7.94244L2.27077e-05 6.05931L46.5532 6.05931L43.2411 1.32834L44.1736 -3.14325e-07L49.075 7.00066L44.1736 14L43.2411 12.6699L46.5532 7.94244Z" fill="#6ED669"/>
              </svg>
          </div>
      </div>
  </article>
     <picture class="about__village__article__picture"
              srcset="
              AboutVillage.png 1025w"
              sizes="(min-width: 1025px) 729px">
         <img src="@/assets/AboutVillage.png"/>
     </picture>
     </div>
     <div class="about__village__info">
         <div class="about__village__info__item">
             <div class="about__village__info__item__smalltext">Площадь земельного участка</div>
             <div class="about__village__info__item__bigtext">
              171 399 m²
             </div>
         </div>
         <div class="about__village__info__item">
             <div class="about__village__info__item__smalltext">Общая застройка</div>
             <div class="about__village__info__item__bigtext">
                 24 460 m²
             </div>
         </div>
         <div class="about__village__info__item">
             <div class="about__village__info__item__smalltext">Количество коттеджей</div>
             <div class="about__village__info__item__bigtext">
                 40
             </div>
         </div>
     </div>
 </section>
</template>
<script>

</script>
<style lang="sass" scoped>
.about__village__section
    display: flex
    flex-direction: column
.about__village__top
    display: flex
    flex-direction: row
.about__village__article
    display: flex
    flex-direction: column
    padding: 58px 0px 0px 116px
.about__village__article__header
    font-style: normal
    font-weight: 700
    font-size: 56px
    line-height: 58px
    letter-spacing: -0.01em
    color: #272727
.about__village__article__header:first-letter
    font-weight: 400
.about__village__article__text
    margin-top: 42px
    p
     font-style: normal
     font-weight: 400
     font-size: 16px
     line-height: 25px
     letter-spacing: -0.01em
     color: #000000
.about__village__article__more
    display: flex
    flex-direction: row
    color: #6ED669
    gap: 18px
    p
     font-style: normal
     font-weight: 500
     font-size: 16px
     line-height: 18px
     letter-spacing: -0.01em
.about__village__article__picture
    padding: 22px 0px 0px 87px
    img
        object-fit: cover
.about__village__info
    display: flex
    flex-direction: row
    padding: 49px 116px 49px 116px
    gap: 50px
.about__village__info__item
    display: flex
    flex-direction: column
.about__village__info__item__bigtext
    background: url("@/assets/row1.png")
    -webkit-background-clip: text
    -webkit-text-fill-color: transparent
    font-style: normal
    font-weight: 800
    font-size: 90px
    line-height: 122px
    display: flex
    align-items: center
    letter-spacing: -0.02em
.about__village__info__item__smalltext
    font-style: normal
    font-weight: 600
    font-size: 14px
    line-height: 22px
    letter-spacing: -0.01em
    color: #000000
.about__village__article__header__items
    display: flex
    flex-direction: row
    gap: 20px
.strelka2
    display: none
.about__village__article__text__mobile
    display: none
@media screen and (max-width: 1024px)
 .about__village__top
    display: flex
    flex-direction: column
 .about__village__article
    display: flex
    flex-direction: column
    padding: 24px 16px 24px 16px
 .about__village__article__picture
    display: none
 .about__village__article__header
    font-style: normal
    font-weight: 700
    font-size: 28px
    line-height: 28px
    letter-spacing: -0.01em
    color: #272727
 .strelka
    display: none
 .strelka2
    display: block
 .about__village__article__text__mobile
    display: block
 .about__village__article__text
    display: none
 .about__village__info
    display: flex
    flex-direction: column
    padding: 40px 16px 40px 16px
    gap: 24px
 .about__village__info__item__bigtext
     font-weight: 800
     font-size: 60px
     height: 98px
     display: flex
     align-items: center
     letter-spacing: -0.02em
     background: url("@/assets/MaskGroup.png")
     -webkit-background-clip: text
     -webkit-text-fill-color: transparent
</style>