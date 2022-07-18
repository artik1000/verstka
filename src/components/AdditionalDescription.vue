<template>
    <section class="additional__description__section">
        <picture class="picture">
            <img src="@/assets/additional.png"/>
        </picture>
        <article class="additional__description__article">
            <h1 class="additional__description__article__header mobile">
                Единство природы<br>
                и истории — основа концепции<br>
                коттеджного поселка<br>
            </h1>
            <div class="additional__description__article__text">
                <p>
                Традиционная русская усадьба - богатейший пласт отечественного<br>
                культурного наследия, гармоничный организм, где природа и<br>
                архитектура сочетаются с поэзией загородной жизни, ее<br>
                экологической целесообразностью.<br>
                <br>
                С русской усадьбой неразрывно связаны имена многих<br>
                государственных деятелей и военачальников, писателей, художников<br>
                - тех, кто составлял веками славу России.
                </p>
            </div>
            <div class="about__village__article__more add">
                <div>
                    <p>Об истории усадьбы</p>
                </div>
                <div class="strelka">
                    <svg width="50" height="14" viewBox="0 0 50 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M46.5532 7.94244L2.26516e-05 7.94244L2.27077e-05 6.05931L46.5532 6.05931L43.2411 1.32834L44.1736 -3.14325e-07L49.075 7.00066L44.1736 14L43.2411 12.6699L46.5532 7.94244Z" fill="#6ED669"/>
                    </svg>
                </div>
            </div>
        </article>
    </section>
</template>
<script>
export default {
    name: 'additional-description'
}
</script>
<style lang="sass" scoped>
.additional__description__section
    display: flex
    flex-direction: row
.additional__description__article
    display: flex
    flex-direction: column
    padding: 79px 141px 0px 52px
.additional__description__article__header
    font-style: normal
    font-weight: 400
    font-size: 42px
    line-height: 50px
    letter-spacing: -0.01em
    color: #000000
.additional__description__article__header::after
    content: "«Усадьба Бергов»"
    font-weight: 700
.additional__description__article__text
    margin-top: 50px
    text-align: left
    p
     font-style: normal
     font-weight: 400
     font-size: 14px
     line-height: 21px
     letter-spacing: -0.01em
     color: #000000
.add
    margin-top: 40px
@media screen and (max-width: 1024px)
    .picture
        display: none
    .additional__description__article
        padding: 0px
    .mobile
        background: url("@/assets/additional.png")
        width: 100vw
        color: white
        font-style: normal
        font-weight: 400
        font-size: 28px
        line-height: 38px
        letter-spacing: -0.01em
        padding: 24px 16px 24px 16px
        background-size: cover
        box-shadow: 100px 100px 100px 100px rgba(0, 0, 0, 0.52) inset
    .additional__description__article__text
        margin-top: 0
        padding: 24px 16px 24px 16px
    .add
      margin-top: 0px
      padding: 16px
    .strelka
      display: none

</style>