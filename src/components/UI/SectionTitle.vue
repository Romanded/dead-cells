<template>
  <div>
    <h2>{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: 'SectionTitle',
  props: {
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
div {
  h2 {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 4em;
    color: #A40239;
    font-family: "Berylium_bd", sans-serif;
    font-weight: normal;

    &:before {
      background: linear-gradient(to right, rgba(164, 2, 57, 0), rgba(164, 2, 57, 0.5));
      display: inline-block;
      height: 3px;
      vertical-align: middle;
      width: 10%;
      content: "";
      font-weight: initial;
    }

    &:after {
      background: linear-gradient(to left, rgba(164, 2, 57, 0), rgba(164, 2, 57, 0.5));
      display: inline-block;
      height: 3px;
      vertical-align: middle;
      width: 10%;
      content: "";
      font-weight: initial;
    }
  }
}
</style>