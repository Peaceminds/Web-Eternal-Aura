<template>
  <section class="pricing-one" id="pricing">
    <div class="container">
      <div class="block-title text-center">
        <h2 class="block-title__title">プレミアム・<span>ビスポークサービス</span>・パッケージ <br></h2><!-- /.block-title__title -->
      </div><!-- /.block-title -->
      <!-- <ul class="list-inline text-center switch-toggler-list" role="tablist" id="switch-toggle-tab">
        <li class="month active"><a href="#">Monthly</a></li>
        <li>
          Rounded switch
          <label class="switch on">
            <span class="slider round"></span>
          </label>
        </li>
        <li class="year"><a href="#">Yearly</a></li>
      </ul> -->
      <!-- /.list-inline -->
      <div class="tabed-content">
        <div id="month">
          <div class="row pricing-one__price-row">
            <div class="col-lg-4 wow fadeInUp" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$3,999</h3>
                <p>basic pack</p>
                <ul class="list-unstyled">
                  <li>パーソナルデザインサービス</li>
                  <li>10年保証</li>
                  <li>1回分の無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 wow fadeInDown" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$6,999</h3>
                <p>medium pack</p>
                <ul class="list-unstyled">
                  <li>職人によるパーソナルなサービス</li>
                  <li>ライフタイム保証</li>
                  <li>3回分の無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 wow fadeInUp" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$39,999</h3>
                <p>premium pack</p>
                <ul class="list-unstyled">
                  <li>プレステージ・デザイン＆ビスポーク・サービス</li>
                  <li>ライフタイム保証</li>
                  <li>ライフタイム無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
          </div><!-- /.row -->
        </div><!-- /#month -->
        <div id="year">
          <div class="row pricing-one__price-row">
            <div class="col-lg-4 wow fadeInUp" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$3,999</h3>
                <p>basic pack</p>
                <ul class="list-unstyled">
                  <li>パーソナルデザインサービス</li>
                  <li>10年保証</li>
                  <li>1回分の無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 wow fadeInDown" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$6,999</h3>
                <p>medium pack</p>
                <ul class="list-unstyled">
                  <li>職人によるパーソナルなサービス</li>
                  <li>ライフタイム保証</li>
                  <li>3回分の無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 wow fadeInUp" data-wow-duration="1500ms">
              <div class="pricing-one__single text-center">
                <h3>$39,999</h3>
                <p>premium pack</p>
                <ul class="list-unstyled">
                  <li>プレステージ・デザイン＆ビスポーク・サービス</li>
                  <li>ライフタイム保証</li>
                  <li>ライフタイム無料メンテナンス</li>
                </ul><!-- /.list-unstyled -->
                <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                <span class="tag-line">No hidden charges!</span>
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
          </div><!-- /.row -->
        </div><!-- /#year -->
      </div><!-- /.tabed-content -->
    </div><!-- /.container -->
  </section>
</template>

<script>
    export default {
      name: "Pricing",
      mounted() {

        function toggleTabWithSwitch() {
          var toggleSwitch = $('#switch-toggle-tab label.switch');
          var monthTabTitle = $('#switch-toggle-tab li.month');
          var yearTabTitle = $('#switch-toggle-tab li.year');
          var monthTabContent = $('#month');
          var yearTabContent = $('#year');
          // hidden show deafult;
          monthTabContent.fadeIn();
          yearTabContent.fadeOut();

          function toggleHandle() {
            if (toggleSwitch.hasClass('on')) {
              yearTabContent.fadeOut();
              monthTabContent.fadeIn();
              monthTabTitle.addClass('active');
              yearTabTitle.removeClass('active');
            } else {
              monthTabContent.fadeOut();
              yearTabContent.fadeIn();
              yearTabTitle.addClass('active');
              monthTabTitle.removeClass('active');
            }
          };
          monthTabTitle.on('click', function() {
            toggleSwitch.addClass('on').removeClass('off');
            toggleHandle();
            return false;
          });
          yearTabTitle.on('click', function() {
            toggleSwitch.addClass('off').removeClass('on');
            toggleHandle();
            return false;
          });
          toggleSwitch.on('click', function() {
            toggleSwitch.toggleClass('on off');
            toggleHandle();
          });

        }
        toggleTabWithSwitch();
      }

    }
</script>

<style scoped>

</style>
