<template>
  <section class="mailchimp-one" id="subscribe">
    <div class="container">
      <div class="block-title text-center">
        <h2 class="block-title__title">Subscribe Our <span>Newsletter</span> <br> to Get New Updates.</h2><!-- /.block-title__title -->
      </div><!-- /.block-title -->
      <form action="#" class="mailchimp-one__mc-form mc-form" data-url="#">
        <input type="email" id="mc-email" class="formInput" placeholder="Email address">
        <button type="submit"><i class="dimon-icon-edit-3"></i>
          <!-- /.fa fa-paper-plane --></button>
      </form><!-- /.mailchimp-one__mc-form -->
      <div class="mc-form__response"></div><!-- /.mc-form__response -->
    </div><!-- /.container -->
  </section>
</template>

<script>
    export default {
      name: "Subscribe"
    }
</script>

<style scoped>

</style>
