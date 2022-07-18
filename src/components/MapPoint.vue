<template>
    <section class="map">
        <div class="map__point">
            <img src="@/assets/Point.png"/>
        </div>
    </section>
</template>
<script>
export default {
    name: 'map-point'
}
</script>
<style lang="sass" scoped>
.map
    background: url('@/assets/map.png')
    height: 428px
.map__point
    position: absolute
    top: 120px
    left: 560px
@media screen and (max-width: 1024px)
  .map
    background-image: url('@/assets/map.png')
    background-size: cover
    background-repeat: no-repeat
    width: 100%
  .map__point
      position: absolute
      top: 100px
      left: 100px
</style>