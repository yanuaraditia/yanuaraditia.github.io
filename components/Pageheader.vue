<template>
  <section class="py-5">
    <b-container>
      <h1 class="title"><span>{{title}}</span></h1>
      <h4 class="subtitle"><span class="text-primary">return</span> $this<span class="text-muted">->{{method}}();</span></h4>
    </b-container>
  </section>
</template>
<script>
export default {
  props: [
    'title',
    'method'
  ]
}
</script>
<style lang="scss" scoped>
.title {
  @media screen and (min-width: 1024px) {
    @keyframes animate {
      0% {
        transform: translateX(-500) skewX(-10deg);
      }
      100% {
        transform: skewX(-10deg) translateX(20px);
      }
    }
    span {
      position: relative;
      &::after {
        content: "";
        width: 4px;
        background: currentColor;
        height: 100%;
        position: absolute;
        transform: skewX(-10deg) translateX(20px);
        animation: animate .4s ease;
      }
    }
  }
}
.subtitle {
  font-weight: 400!important;
}
</style>
