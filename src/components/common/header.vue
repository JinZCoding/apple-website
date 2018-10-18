<template>
    <div class="header_nav">
        <nav class="app_nav">
            <div class="nav_div">
                <ul class="nav_ul">
                    <li class="nav_li"><a href="#" class="nav_a" id="nav_a_apple"><span>index</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>Mac</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>iPad</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>iPhone</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>Watch</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>TV</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>Music</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a"><span>Support</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a" id="nav_a_search"><span>S</span></a></li>
                    <li class="nav_li"><a href="#" class="nav_a" id="nav_a_shop"><span>S</span></a></li>
                </ul>
            </div>
            <div class="nav_div_fold">
                <ul class="nav_main_ul">
                    <li class="nav_items"><a href="javascript:;" @click="showMenu" id="items_list"><span>=</span></a></li>
                    <li class="nav_items"><a href="javascript:;" id="items_index"><span>index</span></a></li>
                    <li class="nav_items"><a href="javascript:;" id="items_shop"><span>shop</span></a></li>
                </ul>
                <div class="menu_search" id="menu_search" v-if="show">
                    <div class="search_inp"></div>
                </div>
                <ul class="nav_menu" id="nav_menu" v-if="show">
                    <li class="menu_items"><a href="javascript:;"><span>Mac</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>iPad</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>iPhone</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>Watch</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>TV</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>Music</span></a></li>
                    <li class="menu_items"><a href="javascript:;"><span>Support</span></a></li>
                </ul>
            </div>
        </nav>
        
    </div>
</template>
<script>
export default {
  data: function() {
    return {
      show: false
    };
  },
  methods: {
    showMenu: function(v) {
      console.log(this.show);
      this.show = !this.show;
    }
  }
};
</script>
<style lang="less">
* {
  margin: 0;
  padding: 0;
  list-style: none;
}
a {
  text-decoration: none;
}
.app_nav {
  position: fixed;
  background-color: rgba(0, 0, 0, 0.8);
  width: 100%;
  z-index: 5;
}
#nav_a_apple,
#nav_a_search,
#nav_a_shop {
  display: inline-block;
  background-size: 16px 44px;
  background-repeat: no-repeat;
  background-image: url(../../../static/image/header_index.svg);
  background-position: center center;
  width: 16px;
  span {
    visibility: hidden;
  }
}
#nav_a_search {
  background-image: url(../../../static/image/header_search.svg);
}
#nav_a_shop {
  background-image: url(../../../static/image/header_shop.svg);
}
#items_index,
#items_shop {
  display: inline-block;
  background-size: 16px 44px;
  background-repeat: no-repeat;
  background-image: url(../../../static/image/header_index.svg);
  background-position: center center;
  width: 16px;
  span {
    visibility: hidden;
  }
}
#items_shop {
  background-image: url(../../../static/image/header_shop.svg);
}
// 导航折叠
@media screen and (max-width: 767px) {
  .nav_div {
    display: none;
  }
  .nav_div_fold {
    font-size: 14px;
    display: block;
    max-width: 980px;
    margin: 0 auto;
    background-color: #000;
    .nav_main_ul {
      display: flex;
      justify-content: space-between;
      padding: 0 22px;
      .nav_items {
        height: 48px;
        line-height: 48px;
        a {
          color: #fff;
        }
      }
    }
    .menu_search {
      position: relative;
      .search_inp {
        // position: absolute;
        height: 38px;
        display: block;
        width: 86%;
        max-width: 584px;
        margin: 0 auto;
        padding: 0;
        background-color: #fff;
        border-radius: 3px;
      }
      &:after {
        position: absolute;
        content: "";
        width: 100%;
        height: 2px;
        color: #fff;
        z-index: 2;
        left: 0;
        right: 0;
        bottom: 0;
      }
    }
    .nav_menu {
      display: block;
      padding: 45px 40px 8px;
      position: relative;
      .menu_items {
        display: block;
        width: 86%;
        max-width: 584px;
        margin: 0px auto;
        height: 44px;
        line-height: 44px;
        // background-color: #fff;
        border-radius: 3px;
        a {
          color: #fff;
          width: auto;
        }
      }
    }
  }
}

@media screen and (min-width: 768px) {
  .nav_div_fold {
    display: none;
  }
  .nav_div {
    font-size: 14px;
    display: block;
    max-width: 980px;
    margin: 0 auto;
    .nav_ul {
      display: flex;
      justify-content: space-between;
      height: 44px;
      line-height: 44px;
      .nav_li {
        width: auto;
        padding: 0 10px;
        // float: left;
        a {
          color: #fff;
        }
      }
    }
  }
}
</style>
