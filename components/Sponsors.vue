<template>
  <section>
    <div class="row">
      <h1 class="title">Sponsors.</h1>
    </div>
    <div class="row center">
      <a class="logo" href="https://github.com">
        <img src="~resources/sponsors/github.svg" />
      </a>
    </div>
    <div class="row">
      <h1 class="title">Supporters.</h1>
    </div>
    <div class="row center">
      <a class="logo" href="https://ussu.co.uk/">
        <img src="~resources/sponsors/union.svg" />
      </a>
    </div>
    <div class="row center">
      <h1><a class="button" href="mailto:sponsor@hacksurrey.uk">Become a sponsor!</a></h1>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
section
  display: flex
  flex-wrap: wrap
  min-width: 96%
  padding: 1.5em 2em
  flex-direction: column
  justify-content: left

.row
  padding: .5em 1.5em
  margin: .5em .75em
  display: flex
  flex: 1 1 auto
  h1
    padding: 0
    color: #FF3232
    font-size: 3.5em
    font-weight: 500
    margin: 0 0 5px 0

.center
  justify-content: center

.logo
  display: flex
  align-items:  center
  padding: 0 1.5em

img
  width: 42vw
  max-height: 70px
  min-width: 200px
  max-width: 400px

.button
  font-size: 1.1rem
  // font-size: 20px
</style>
