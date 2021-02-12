<template>
  <section class="py-lg-5">
    <b-container class="py-lg-5 front-banner">
      <b-row>
        <div class="order-1 col-lg-6 order-lg-0">
          <img src="~/assets/me.jpg" alt="" class="radius-100 mb-3">
          <h1>Hello, i am Yanuar Aditia.</h1>
          <p>I am an software developer and the backend team of <a href="//kiriminaja.com">KiriminAja.com</a>.
            Sometimes my work is open source and publicly available on github.
            You can follow me at <a href="//t.me/yanuaraditia">Telegram</a> where I mostly learning about backend technology.
          </p>
          <p>Outside of programming and creating new features, I enjoy video games, boba tea and customize my phone</p>
        </div>
        <div class="order-0 col-lg-auto order-lg-1">
        </div>
      </b-row>
    </b-container>
  </section>
</template>
<style lang="scss" scoped>
.front-banner {
  @media screen and (min-width: 1024px) {
    h1 {
      font-size: 3rem;
    }
    img {
      max-width: 170px;
    }
    p {
      font-size: 1.4rem;
    }
  }
  @media screen and (max-width: 1023px) {
    img {
      max-width: 100%;
      height: auto;
    }
  }
}
</style>
<script>
export default {
  head: {
    title: 'Home'
  }
}
</script>
