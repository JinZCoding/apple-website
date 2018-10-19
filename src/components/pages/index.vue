<template>
    <div>
        <Header></Header>
        <div class="content">
            <div class="con_top">
                <div class="con_newpro con_one">
                    <div class="chardetail">
                        <h2>
                            <span>iPhone XS</span>
                        </h2>
                        <h3>Welcome to the big screens.</h3>
                        <div class="conlink">
                            <a href="#">Learn more</a>
                            <a href="#">Buy</a>
                        </div>
                    </div>
                    <div class="img_cover">
                        <figure class="html_img"></figure>
                    </div>
                </div>
                <div class="con_newpro con_two">
                    <div class="chardetail">
                      <h2>
                        <span>iPhone XR</span>
                      </h2>
                      <h3>Brilliant.In every way.</h3>
                      <p>Pre-order 10.19</p>
                    </div>
                    <div class="img_cover">
                        <figure class="html_img"></figure>
                    </div>
                </div>
                <div class="con_newpro con_three">
                    <div class="chardetail">
                      <h2>
                        <span>WATCH</span>
                      </h2>
                      <h3>All new.For a better you.</h3>
                      <div class="conlink">
                          <a href="#">Learn more</a>
                          <a href="#">Buy</a>
                      </div>
                    </div>
                    <div class="img_cover">
                        <figure class="html_img"></figure>
                    </div>
                </div>
            </div>         
            <div class="con_bot">
                <div class="bot_items" id="imgcover_one">
                  <div class="bot_detail">
                    <h4><span>Apple Special Event</span></h4>
                    <h5>Live from Brooklyn.Watch on October 30 at 10 a.m.EDT.</h5>
                  </div>
                  <div class="botimg_cover">
                    <figure></figure>
                  </div>
                </div>
                <div class="bot_items" id="imgcover_two">
                  <div class="bot_detail">
                    <h4><span>Apple GiveBack</span></h4>
                    <h5>Trade in your old device for credit toward a new one.</h5>
                    <div class="bot_link">
                      <a href="#">See how it works</a>
                    </div>
                  </div>
                  <div class="botimg_cover" >
                    <figure></figure>
                  </div>
                </div>
                <div class="bot_items" id="imgcover_three">
                  <div class="bot_detail">
                    <h4><span>Music</span></h4>
                    <h5>Lose yourself in 50 million songs.</h5>
                    <div class="bot_link">
                      <a href="#">Try it free*</a>
                      <a href="#">Learn More</a>
                    </div>
                  </div>
                  <div class="botimg_cover">
                    <figure></figure>
                  </div>
                </div>
                <div class="bot_items" id="imgcover_four">
                  <div class="bot_detail">
                    <h4><span>AirPods</span></h4>
                    <h5>Wireless.Effortless.Magical.</h5>
                    <div class="bot_link">
                      <a href="#">Learn More</a>
                      <a href="#">Buy</a>
                    </div>
                  </div>
                  <div class="botimg_cover" >
                    <figure></figure>
                  </div>
                </div>
                <div class="bot_items" id="imgcover_five">
                  <div class="bot_detail">
                    <h4><span>MacBook Pro</span></h4>
                    <h5>More power.More Performance.More pro.</h5>
                    <div class="bot_link">
                      <a href="#">Learn More</a>
                      <a href="#">Buy</a>
                    </div>
                  </div>
                  <div class="botimg_cover" >
                    <figure></figure>
                  </div>
                </div>
                <div class="bot_items" id="imgcover_six">
                  <div class="bot_detail">
                    <h4><span>iPad</span></h4>
                    <h5>Like a computer.Unlike any computer.</h5>
                    <div class="bot_link">
                      <a href="#">Learn More</a>
                      <a href="#">Buy</a>
                    </div>
                  </div>
                  <div class="botimg_cover" >
                    <figure></figure>
                  </div>
                </div>
            </div>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from "@/components/common/header";
import Footer from "@/components/common/footer";
export default {
  components: {
    Header,
    Footer
  }
};
</script>
<style lang="less">
.content {
  position: relative;
  .con_top {
    padding-top: 44px;
    .con_newpro {
      cursor: pointer;
      width: 100%;
      height: 580px;
      margin-bottom: 10px;
      position: relative;
      .chardetail {
        text-align: center;
        padding-top: 47px;
        h2 {
          background-repeat: no-repeat;
          background-position: center;
          font-size: 56px;
          line-height: 56px;
          font-weight: 600;
          overflow: hidden;
          text-align: center;
          display: block;
          span {
            visibility: hidden;
          }
        }
        .conlink {
          display: inline-block;
          font-size: 19px;
          line-height: 28px;
          margin-top: 10px;
          a {
            color: #6bf;
            &:after {
              content: ">";
              padding-left: 3px;
              text-decoration: none;
            }
            &:hover {
              text-decoration: underline;
            }
          }
        }
      }
    }
    // 商品1，2的样式与3不同
    .con_one,
    .con_two {
      background-color: #000;
      .chardetail {
        color: #fff;
      }
      .img_cover {
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        overflow: hidden;
        .html_img {
          z-index: 1;
          position: absolute;
          border: 0;
          margin: 0;
          padding: 0;
          left: calc(50% + 0px);
          right: auto;
          bottom: 0px;
          top: auto;
          -webkit-transform: translatex(-50%);
          transform: translatex(-50%);
        }
      }
    }
    .con_three {
      height: 570px;
      background-color: rgb(250, 250, 250);
      .chardetail {
        color: #000;
        .conlink {
          a {
            color: #0070c9;
          }
        }
      }
    }
  }
}

@media screen and (max-width: 681px) {
  .con_top{
    .chardetail {
      h3 {
        font-size: 19px;
        line-height: 36px;
        font-weight: 400;
      }
    }
    .con_one {
      h2 {
        background-image: url(../../../static/image/iphone_xs_logo_hero_small.png);
      }
      .img_cover {
        .html_img {
          width: 200px;
          height: 331px;
          margin: 60px auto;
          background-size: 200px 331px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xs_small.jpg);
        }
      }
    }
    .con_two {
      h2 {
        background-image: url(../../../static/image/iphone_xr_logo_hero_small.png);
      }
      .img_cover {
        .html_img {
          width: 216px;
          height: 332px;
          margin: 60px auto;
          background-size: 216px 332px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xr_small.jpg);
        }
      }
    }
    .con_three {
      h2 {
        height: 47px;
        background-image: url(../../../static/image/apple_watch_series_4_logo_hero_small.jpg);
      }
      .img_cover {
        .html_img {
          width: 422px;
          height: 309px;
          margin: 60px auto;
          background-size: 422px 309px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/apple_watch_series_4_small.jpg);
        }
      }
    }
  }
}

@media screen and (min-width: 682px) and (max-width: 1027px) {
  .con_top{
    .chardetail {
      h3 {
        font-size: 24px;
        line-height: 36px;
        font-weight: 400;
      }
    }
    .con_one {
      h2 {
        background-image: url(../../../static/image/iphone_xs_logo_hero_medium.png);
      }
      .img_cover {
        .html_img {
          width: 682px;
          height: 315px;
          margin: 60px auto;
          background-size: 682px 315px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xs_medium.jpg);
        }
      }
    }
    .con_two {
      h2 {
        background-image: url(../../../static/image/iphone_xr_logo_hero_medium.png);
      }
      .img_cover {
        .html_img {
          width: 890px;
          height: 321px;
          margin: 60px auto;
          background-size: 890px 321px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xr_medium.jpg);
        }
      }
    }
    .con_three {
      // text-align: center;
      padding-top: 47px;
      height: 569px;
      margin-bottom: 10px;
      position: relative;
      .chardetail {
        display: inline-block;
        position: absolute !important;
        width: 50%;
        top: 50%;
        right: 50%;
        -webkit-transform: translateY(-50%);
        transform: translateY(-50%);
        padding-top: 0;
      }
      h2 {
        height: 55px;
        background-image: url(../../../static/image/apple_watch_series_4_logo_hero_medium.jpg);
      }
      .img_cover {
        .html_img {
          width: 339px;
          height: 617px;
          // margin: 50px 0 0 auto;
          background-size: 339ppx;
          background-repeat: no-repeat;
          position: absolute;
          left: 50%;
          width: 50%;
          margin-left: 0;
          top: 0;
          background-image: url(../../../static/image/apple_watch_series_4_medium.jpg);
        }
      }
    }
  }
}

@media screen and (min-width: 1028px) {
  .con_top{
    .chardetail {
      h3 {
        font-size: 27px;
        line-height: 38px;
        font-weight: 400;
      }
    }
    .con_one {
      h2 {
        background-image: url(../../../static/image/iphone_xs_logo_hero_large.png);
      }
      .img_cover {
        .html_img {
          width: 972px;
          height: 337px;
          margin: 50px auto;
          background-size: 972px 337px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xs_large.jpg);
        }
      }
    }
    .con_two {
      h2 {
        background-image: url(../../../static/image/iphone_xr_logo_hero_large.png);
      }
      .img_cover {
        .html_img {
          width: 986px;
          height: 358px;
          margin: 50px auto;
          background-size: 986px 358px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/iphone_xr_large.jpg);
        }
      }
    }
    .con_three {
      // text-align: center;
      padding-top: 47px;
      height: 569px;
      margin-bottom: 10px;
      position: relative;
      overflow: hidden;
      .chardetail {
        display: inline-block;
        position: absolute !important;
        width: 50%;
        top: 50%;
        right: 50%;
        -webkit-transform: translateY(-50%);
        transform: translateY(-50%);
        padding-top: 0;
      }
      h2 {
        height: 78px;
        background-image: url(../../../static/image/apple_watch_series_4_logo_hero_large.jpg);
      }
      .img_cover {
        overflow: hidden;
        .html_img {
          width: 340px;
          height: 624px;
          // margin: 50px 0 0 auto;
          background-size: 340px 624px;
          background-repeat: no-repeat;
          position: absolute;
          left: 50%;
          width: 50%;
          margin-left: 0;
          top: 0;
          background-image: url(../../../static/image/apple_watch_series_4_large.jpg);
        }
      }
    }
  }
  .con_bot{
    .bot_items{
      height: 580px;
      .bot_detail{
        h4{
          margin-top: 60px;
          font-size: 36px;
          line-height: 44px;
          font-weight: 600;
        }
        h5{
          font-size: 19px;
          line-height: 23px;
        }
      }
    }
    #imgcover_one {
      .botimg_cover {
        figure {
          width: 1262px;
          height: 580px;
          background-size: 1262px 580px;
          background-image: url(../../../static/image/special_event_7__difpjxgizggi_large.jpg);
        }
      }
    }
    #imgcover_two {
      .botimg_cover {
        figure {
          width: 1262px;
          height: 580px;
          background-size: 1262px 580px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/give_back_large.jpg);
        }
      }
    }
    #imgcover_three {
      .bot_detail {
        color: #fafafa;
        .bot_link {
          a {
            color: #fafafa;
          }
        }
      }
      .botimg_cover {
        figure {
          width: 1262px;
          height: 580px;
          background-size: 1262px 580px;
          background-image: url(../../../static/image/apple_music_large.jpg);
          }
      }
    }
    #imgcover_four {
      .botimg_cover {
        figure {
          width: 417px;
          height: 387px;
          background-size: 417px 387px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/airpods_large.jpg);
          
        }
      }
    }
    #imgcover_five {
      .bot_detail {
        color: #fafafa;
      }
      .botimg_cover {
        figure {
          width: 1262px;
          height: 580px;
          background-size: 1262px 580px;
          background-image: url(../../../static/image/macbook_pro_performance_large.jpg);
          }
      }
    }
    #imgcover_six {
      .botimg_cover {
        figure {
          width: 516px;
          height: 335px;
          background-size: 516px 335px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/ipad_large.jpg);
          
        }
      }
    }
  }
}

@media screen and (max-width: 735px) {
  .con_bot{
    width: 100%;
    display: flex;
    flex-flow: column;
    .bot_items{
      box-sizing: border-box;
      width: 100%;
      border-left-width: 0;
      border-right-width: 0;
      box-sizing: border-box;
      position: relative;
      height: 500px;
      background-color: #fafafa;
      border-color: #fff;
      border-style: solid;
      border-top-width: 6px;
      border-bottom-width: 6px;
      overflow: hidden;
      .bot_detail {
        text-align: center;
        z-index: 4;
        position: relative;
        h4 {
          margin-top: 37px;
          font-size: 32px;
          line-height: 38px;
          font-weight: 600;
          width: 88%;
          max-width: 430px;
          margin-left: auto;
          margin-right: auto;
          text-align: center;
        }
        h5 {
          text-align: center;
          width: 88%;
          max-width: 430px;
          font-size: 19px;
          line-height: 23px;
          font-weight: 200;
          letter-spacing: 0.02em;
          margin-top: 4px;
          margin-left: auto;
          margin-right: auto;
        }
        .bot_link {
          a {
            color: rgb(0, 112, 201);
            font-size: 17px;
            font-weight: 400;
            // height: 21px;
            &:hover {
              text-decoration: underline;
            }
            &:after {
              content: ">";
            }
          }
        }
      }
      .botimg_cover {
        z-index: 1;
        overflow: visible;
        flex-flow: 1;
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        figure {

          z-index: 1;
          position: absolute;
          border: 0;
          margin: 0;
          padding: 0;
          left: calc(50% + 0px);
          right: auto;
          bottom: 0px;
          top: auto;
          -webkit-transform: translatex(-50%);
          transform: translatex(-50%);
        }
      }
    }
    #imgcover_one {
      .botimg_cover {
        figure {
          width: 736px;
          height: 548px;
          background-size: 736px 548px;
          background-image: url(../../../static/image/special_event_7__difpjxgizggi_small.jpg);
        }
      }
    }
    #imgcover_two {
      .botimg_cover {
        figure {
          width: 736px;
          height: 548px;
          background-size: 736px 548px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/give_back_small.jpg);
        }
      }
    }
    #imgcover_three {
      .bot_detail {
        color: #fafafa;
        .bot_link {
          a {
            color: #fafafa;
          }
        }
      }
      .botimg_cover {
        figure {
          width: 736px;
          height: 548px;
          background-size: 736px 548px;
          background-image: url(../../../static/image/apple_music_small.jpg);
          }
      }
    }
    #imgcover_four {
      .botimg_cover {
        figure {
          width:304px;
          height: 314px;
          background-size: 304px 314px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/airpods_medium.jpg);
          
        }
      }
    }
    #imgcover_five {
      .bot_detail {
        color: #fafafa;
      }
      .botimg_cover {
        figure {
          width: 736px;
          height: 548px;
          background-size: 736px 548px;
          background-image: url(../../../static/image/macbook_pro_performance_small.jpg);
          }
      }
    }
    #imgcover_six {
      .botimg_cover {
        figure {
          width: 228px;
          height: 340px;
          background-size: 228px 340px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/ipad_small.jpg);
          
        }
      }
    }
  }
}
@media screen and (min-width: 736px){
  .con_bot {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    width: 100%;
    // position: relative;
    .bot_items {
      box-sizing: border-box;
      position: relative;
      // height: 580px;
      width: 50%;
      background-color: #fafafa;
      border-color: #fff;
      border-style: solid;
      border-top-width: 6px;
      border-bottom-width: 6px;
      overflow: hidden;
      .bot_detail {
        text-align: center;
        z-index: 4;
        position: relative;
        h4 {
          // font-size: 36px;
          // line-height: 44px;
          // font-weight: 600;
          width: 88%;
          max-width: 430px;
          margin-left: auto;
          margin-right: auto;
          text-align: center;
        }
        h5 {
          text-align: center;
          width: 88%;
          max-width: 430px;
          // font-size: 19px;
          // line-height: 23px;
          font-weight: 200;
          letter-spacing: 0.02em;
          margin-top: 4px;
          margin-left: auto;
          margin-right: auto;
        }
        .bot_link {
          a {
            color: rgb(0, 112, 201);
            font-size: 17px;
            font-weight: 400;
            // height: 21px;
            &:hover {
              text-decoration: underline;
            }
            &:after {
              content: ">";
            }
          }
        }
      }
      .botimg_cover {
        z-index: 1;
        overflow: visible;
        flex-flow: 1;
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        figure {
          z-index: 1;
          position: absolute;
          border: 0;
          margin: 0;
          padding: 0;
          left: calc(50% + 0px);
          right: auto;
          bottom: 0px;
          top: auto;
          -webkit-transform: translatex(-50%);
          transform: translatex(-50%);
        }
      }
      &:nth-child(2n + 1) {
        border-left-width: 12px;
      }
      &:nth-child(2n) {
        border-right-width: 12px;
      }
    }
  }
}
@media screen and (min-width: 736px) and (max-width: 1027px) {
  .con_bot{
    .bot_items{
      height: 490px;
      .bot_detail{
        h4{
          margin-top: 50px;
          font-size: 32px;
          line-height: 36px;
          font-weight: 400;
        }
        h5{
          font-size: 19px;
          line-height: 23px;
        }
      }
    }
    #imgcover_one {
      .botimg_cover {
        figure {
          width: 516px;
          height: 490px;
          background-size: 516px 490px;
          background-image: url(../../../static/image/special_event_7__difpjxgizggi_medium.jpg);
        }
      }
    }
    #imgcover_two {
      .botimg_cover {
        figure {
          width: 516px;
          height: 490px;
          background-size: 516px 490px;
          background-image: url(../../../static/image/give_back_medium.jpg);
        }
      }
    }
    #imgcover_three {
      .bot_detail {
        color: #fafafa;
        .bot_link {
          a {
            color: #fafafa;
          }
        }
      }
      .botimg_cover {
        figure {
          width: 516px;
          height: 490px;
          background-size: 516px 490px;
          background-image: url(../../../static/image/apple_music_medium.jpg);
          }
      }
    }
    #imgcover_four {
      .botimg_cover {
        figure {
          width: 304px;
          height: 314px;
          background-size: 304px 314px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/airpods_medium.jpg);
          
        }
      }
    }
    #imgcover_five {
      .bot_detail {
        color: #fafafa;
      }
      .botimg_cover {
        figure {
          width: 516px;
          height: 490px;
          background-size: 516px 490px;
          background-image: url(../../../static/image/macbook_pro_performance_medium.jpg);
          }
      }
    }
    #imgcover_six {
      .botimg_cover {
        figure {
          width: 228px;
          height: 320px;
          background-size: 228px 320px;
          background-repeat: no-repeat;
          background-image: url(../../../static/image/ipad_medium.jpg);
          
        }
      }
    }
  }
}

</style>
