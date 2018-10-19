<template>
    <div class="footer">
        <div class="outer">
            <div class="top_ban">
                <ul>
                    <li>* New subscribers only. Plan automatically renews after trial.</li>
                </ul>
            </div>
            <nav class="mid_ban">
                <!-- Shop and Learn -->
                <div class="mid_item">
                    <label>
                        <h3>Shop and Learn</h3>
                    </label>
                    <ul>
                        <li>Mac</li>
                        <li>iPad</li>
                        <li>iPhone</li>
                        <li>Watch</li>
                        <li>TV</li>
                        <li>Music</li>
                        <li>iTunes</li>
                        <li>HomePod</li>
                        <li>iPod touch</li>
                        <li>Accessories</li>
                        <li>Gift Carda</li>
                    </ul>
                </div>
                <!-- Apple Store -->
                <div class="mid_item">
                    <label><h3>Apple Store</h3></label>
                    <ul>
                        <li>Find a Store</li>
                        <li>Genius Bar</li>
                        <li>Today at Apple</li>
                        <li>Apple Camp</li>
                        <li>Field Trip</li>
                        <li>Apple Store App</li>
                        <li>Refurbished and Clearance</li>
                        <li>Financing</li>
                        <li>Apple GiveBack</li>
                        <li>Order Status</li>
                        <li>Shopping Help</li>
                    </ul>
                </div>
                <!-- For Education   For Business -->
                <div class="mid_item">
                    <div>
                        <label><h3>For Education</h3></label>
                        <ul>
                            <li>Apple and Education</li>
                            <li>Shop for College</li>
                        </ul>
                    </div>
                    <div>
                        <label><h3>For Business</h3></label>
                        <ul>
                            <li>Apple and Business</li>
                            <li>Shop for Business</li>
                        </ul>
                    </div>
                </div>
                <!-- Account   Apple Values -->
                <div class="mid_item">
                    <div>
                        <label><h3>Account</h3></label>
                        <ul>
                            <li>Manage Your Apple ID</li>
                            <li>Apple Store Account</li>
                            <li>iCloud.com</li>
                        </ul>
                    </div>
                    <div>
                        <label><h3>Apple Values</h3></label>
                        <ul>
                            <li>Accessibility</li>
                            <li>Education</li>
                            <li>Environment</li>
                            <li>Inclusion and Diversity</li>
                            <li>Privacy</li>
                            <li>Supplier Responsibility</li>
                        </ul>
                    </div>
                </div>
                <!-- About Apple -->
                <div class="mid_item">
                    <label><h3>About Apple</h3></label>
                    <ul>
                        <li>Newsroom</li>
                        <li>Apple Leadership</li>
                        <li>Job Opportunities</li>
                        <li>Investors</li>
                        <li>Events</li>
                        <li>Contact Apple</li>
                    </ul>
                </div>
            </nav>
            <nav class="minmid_ban">
                <div class="minnav_div">
                    <div class="cshow" @click="s1 = !s1">
                        <a href="javascript:;" v-if="!s1"><span>+</span></a>
                        <a href="javascript:;" v-if="s1"><span>x</span></a>
                        <div class="min_tit">
                            <span>Shop and Learn</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s1">
                        <li><a href="javascript:;">Mac</a></li>
                        <li><a href="javascript:;">iPad</a></li>
                        <li><a href="javascript:;">iPhone</a></li>
                        <li><a href="javascript:;">Watch</a></li>
                        <li><a href="javascript:;">TV</a></li>
                        <li><a href="javascript:;">Music</a></li>
                        <li><a href="javascript:;">iTunes</a></li>
                        <li><a href="javascript:;">HomePod</a></li>
                        <li><a href="javascript:;">iPod touch</a></li>
                        <li><a href="javascript:;">Accessories</a></li>
                        <li><a href="javascript:;">Gift Carda</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s2 = !s2">
                        <a href="javascript:;" v-if="!s2"><span>+</span></a>
                        <a href="javascript:;" v-if="s2"><span>x</span></a>
                        <div class="min_tit">
                            <span>Apple Store</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s2">
                        <li><a href="javascript:;">Find a Store</a></li>
                        <li><a href="javascript:;">Genius Bar</a></li>
                        <li><a href="javascript:;">Today at Apple</a></li>
                        <li><a href="javascript:;">Apple Camp</a></li>
                        <li><a href="javascript:;">Field Trip</a></li>
                        <li><a href="javascript:;">Apple Store App</a></li>
                        <li><a href="javascript:;">Refurbished and Clearance</a></li>
                        <li><a href="javascript:;">Financing</a></li>
                        <li><a href="javascript:;">Apple GiveBack</a></li>
                        <li><a href="javascript:;">Order Status</a></li>
                        <li><a href="javascript:;">Shopping Help</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s3 = !s3">
                        <a href="javascript:;" v-if="!s3"><span>+</span></a>
                        <a href="javascript:;" v-if="s3"><span>x</span></a>
                        <div class="min_tit">
                            <span>For Education</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s3">
                        <li><a href="javascript:;">Apple and Education</a></li>
                        <li><a href="javascript:;">Shop for College</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s4 = !s4">
                        <a href="javascript:;" v-if="!s4"><span>+</span></a>
                        <a href="javascript:;" v-if="s4"><span>x</span></a>
                        <div class="min_tit">
                            <span>For Business</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s4">
                        <li><a href="javascript:;">Apple and Business</a></li>
                        <li><a href="javascript:;">Shop for Business</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s5 = !s5">
                        <a href="javascript:;" v-if="!s5"><span>+</span></a>
                        <a href="javascript:;" v-if="s5"><span>x</span></a>
                        <div class="min_tit">
                            <span>Account</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s5">
                        <li><a href="javascript:;">Manage Your Apple ID</a></li>
                        <li><a href="javascript:;">Apple Store Account</a></li>
                        <li><a href="javascript:;">iCloud.com</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s6 = !s6">
                        <a href="javascript:;" v-if="!s6"><span>+</span></a>
                        <a href="javascript:;" v-if="s6"><span>x</span></a>
                        <div class="min_tit">
                            <span>Apple Values</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s6">
                        <li><a href="javascript:;">Accessibility</a></li>
                        <li><a href="#">Education</a></li>
                        <li><a href="#">Environment</a></li>
                        <li><a href="#">Inclusion and Diversity</a></li>
                        <li><a href="#">Privacy</a></li>
                        <li><a href="#">Supplier Responsibility</a></li>
                    </ul>
                </div>
                <div class="minnav_div">
                    <div class="cshow" @click="s7 = !s7">
                        <a href="javascript:;" v-if="!s7"><span>+</span></a>
                        <a href="javascript:;" v-if="s7"><span>x</span></a>
                        <div class="min_tit">
                            <span>About Apple</span>
                        </div>
                    </div>
                    <ul class="min_items" v-if="s7">
                        <li><a href="#">Newsroom</a></li>
                        <li><a href="#">Apple Leadership</a></li>
                        <li><a href="#">Job Opportunities</a></li>
                        <li><a href="#">Investors</a></li>
                        <li><a href="#">Events</a></li>
                        <li><a href="#">Contact Apple</a></li>
                    </ul>
                </div>
            </nav>
            <div class="bot_ban">
                <div class="more_ways">
                    More ways to shop: Visit an <a href="#">Apple Store</a>, call 1-800-MY-APPLE, or <a href="#">find a reseller</a>.
                </div>
                <div class="usico"><span></span>United States</div>
                <div class="app_copy">
                    <div class="copy_info">Copyright &copy; 2018 Apple Inc. All rights reserved.</div>
                    <div class="copy_link">
                        <a href="#">Privacy Policy</a>
                        <a href="#">Terms of Use</a>
                        <a href="#">Sales and Refunds</a>
                        <a href="#">Legal</a>
                        <a href="#">Site Map</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
  data() {
    return {
      s1: false,
      s2: false,
      s3: false,
      s4: false,
      s5: false,
      s6: false,
      s7: false
    };
  },
  methods: {}
};
</script>
<style lang="less">
.footer {
  //   text-align: center;
  background-color: #f2f2f2;
  font-size: 12px;
  line-height: 24px;
  color: #888;
  h3 {
    color: #333;
    font-size: 12px;
  }
  .outer {
    margin: 0 auto;
    max-width: 980px;
    padding: 0 22px;
    .top_ban {
      border-bottom: 1px solid #d6d6d6;
      color: #888;
      padding: 17px 0 11px;
    }
    .mid_ban {
      position: relative;
      padding-top: 20px;
      overflow: hidden;
      .mid_item {
        position: relative;
        width: 20%;
        float: left;
      }
    }
    .minmid_ban {
      position: relative;
      padding-top: 14px;
      overflow: hidden;
      cursor: pointer;
      .minnav_div {
        a {
          color: #333;
        }
        padding-bottom: 5px;
        border-bottom: 1px solid #d6d6d6;
        // &:last-child {
        //   border-bottom: none;
        // }
        .min_tit {
          padding: 6px 0 4px;
          span {
            font-size: 12px;
            color: #333;
          }
        }
        .min_items {
          // display: none;
          li {
            line-height: 26px;
            padding-left: 24px;
            a {
              display: block;
              font-size: 12px;
              color: #888;
              float: none;
              &:hover {
                text-decoration: underline;
              }
            }
          }
        }
        a {
          float: right;
        }
      }
    }
    .bot_ban {
      padding: 17px 0 21px;
      padding-top: 15px;
      border-top: none;
      .more_ways {
        padding-bottom: 5px;
        border-bottom: 1px solid #d6d6d6;
        a {
          color: #0070c9;
        }
      }
      .usico {
        // float: right;
        margin-top: 5px;
        position: relative;
        top: -3px;
        z-index: 2;
        // white-space: nowrap;
        span {
          display: inline-block;
          width: 16px;
          height: 16px;
          background-repeat: no-repeat;
          background-size: 16px 16px;
          background-image: url(../../../static/image/16.png);
          padding-right: 5px;
          background-position: left center;
          cursor: pointer;
          //   float: left;
          //   margin-top: -1px;
        }
      }
      .copy_link {
        a {
          color: rgb(85, 85, 85);
          padding: 0 12px 0;
          border-right: 1px solid #d6d6d6;
          &:first-child {
            padding-left: 0;
          }
          &:last-child {
            border-right: none;
          }
        }
      }
    }
  }
}
@media screen and (max-width: 767px) {
  .mid_ban {
    display: none;
  }
  .minmid_ban {
    display: block;
  }
}
@media screen and (min-width: 768px) {
  .mid_ban {
    display: block;
  }
  .minmid_ban {
    display: none;
  }
  .bot_ban {
    .usico {
      float: right;
    }
  }
}
</style>
