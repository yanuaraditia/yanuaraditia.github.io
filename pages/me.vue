<template>
  <div>
    <Pageheader title="Something just like this" method="me"/>
    <section>
      <b-container>
        <b-row>
          <div class="col-lg-8">
            <p>My full name is Yanuar Aditia, and Yanuar in short. Born, raised, and currently living in Yogyakarta, Indonesia. Currently working as Backend Developer at Tries Company Yogyakarta.</p>
            <p>I start getting into web dev on high school by creating an blog/CMS for practicum management using native PHP, then learning various php framework like CI, CakePHP, Yii, but now I'd prefer using Laravel.</p>
            <p>Nowadays I spend my time to organize IMAKA site, sometimes hang around various programming/web dev user groups, play some games, and keep learning new things while I can.</p>
            <p>You can contact me via email at <a href="mailto:yanuaraditia@outlook.com">yanuaraditia@outlook.com</a>.</p>
            <b-row class="g-3">
              <div class="col-lg-4">
                <strong class="text-primary">Age : </strong><span>{{myAge}}</span>
              </div>
              <div class="col-lg-4">
                <strong class="text-primary">Residence : </strong><span>Indonesia</span>
              </div>
              <div class="col-lg-4">
                <strong class="text-primary">Freelance : </strong><span>Available</span>
              </div>
              <div class="col-lg-4">
                <strong class="text-primary">Address : </strong><span>Yogyakarta, ID</span>
              </div>
              <div class="col-lg-4">
                <strong class="text-primary">Chat : </strong><a class="text-white" href="//t.me/yanuaraditia">t.me/yanuaraditia</a>
              </div>
              <div class="col-lg-4">
                <strong class="text-primary">Mail : </strong><a class="text-white" href="mailto:yanuaraditia@outlook.com">yanuaraditia@outlook.com</a>
              </div>
            </b-row>
          </div>
        </b-row>
      </b-container>
    </section>
    <section class="py-5">
      <b-container>
        <h3 class="title is-5 has-text-primary">Coding Skills</h3>
        <b-row class="g-3">
          <div class="col-lg-6">
            <small>PHP / Laravel</small>
            <b-progress :value="95" show-value format="percent" variant="primary"></b-progress>
          </div>
          <div class="col-lg-6">
            <small>HTMl,CSS,SASS</small>
            <b-progress :value="85" show-value format="percent" variant="primary"></b-progress>
          </div>
          <div class="col-lg-6">
            <small>Javascript / VueJS</small>
            <b-progress :value="75" show-value format="percent" variant="primary"></b-progress>
          </div>
          <div class="col-lg-6">
            <small>SQL / MySQL</small>
            <b-progress :value="85" show-value format="percent" variant="primary"></b-progress>
          </div>
        </b-row>
      </b-container>
    </section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: 'About me'
    }
  },
  computed: {
    myAge() {
      let currentDate = new Date();
      let birthDate = new Date("1999/01/07");
      let difference = currentDate - birthDate;
      let age = Math.floor(difference/31557600000);
      return age
    }
  }
}
</script>
