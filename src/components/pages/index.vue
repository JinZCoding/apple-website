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
            <!-- <div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#"></a><a href="#"></a>
                </div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#">Learn More ></a><a href="#">Buy ></a>
                </div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#"></a><a href="#"></a>
                </div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#">Learn More ></a><a href="#">Buy ></a>
                </div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#">Learn More ></a><a href="#">Buy ></a>
                </div>
                <div>
                    <h2></h2>
                    <p></p>
                    <a href="#">Learn More ></a><a href="#">Buy ></a>
                </div>
            </div> -->
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
          // font-size: 21px;
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
  .chardetail {
    h2 {
      background-repeat: no-repeat;
      background-position: center;
    }
    h3 {
      font-size: 19px;
      line-height: 36px;
      font-weight: 400;
    }
    .conlink {
      font-size: 19px;
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
@media screen and (min-width: 682px) and (max-width: 1027px) {
  .chardetail {
    h2 {
      background-repeat: no-repeat;
      background-position: center;
    }
    h3 {
      font-size: 24px;
      line-height: 36px;
      font-weight: 400;
    }
    .conlink {
      font-size: 21px;
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
  }
  .con_three {
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
@media screen and (min-width: 1028px) {
  .chardetail {
    h2 {
      background-repeat: no-repeat;
      background-position: center;
    }
    h3 {
      font-size: 27px;
      line-height: 38px;
      font-weight: 400;
    }
    .conlink {
      font-size: 21px;
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
  }
  .con_three {
    h2 {
      height: 78px;
      background-image: url(../../../static/image/apple_watch_series_4_logo_hero_large.jpg);
    }
    .img_cover {
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
</style>
