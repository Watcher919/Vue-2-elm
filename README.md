# 前言

初学vue时曾在网上搜索vue的实战项目源码，无奈大部分都是简单的demo，对于深究vue没有太大的帮助，剩下的一些大部分都是像音乐播放器之类的展示型项目，交互没有预期那么复杂。但我们实际在工作中，经常会遇到有购物车的项目，这类项目因为涉及到money，所以对逻辑严谨度要求高，页面之间交互复杂，又会伴随着登录、注册、用户信息等等，常常会让我们很头疼。既然还没人用vue写过这样的项目，那不如我来写，开源出来对能看到的人也会有帮助。

这种功能性的项目很实用但是往往也很枯燥，没有音乐播放器那么看起来绚丽，思来想去发现饿了么是一个不错的素材，一来它足够复杂，开放的外卖平台比一般的公司独有商店更加复杂。二来 见到那么多美食，大家也不会感觉到厌烦。

为啥是饿了么，而不是百度，美团？原因很简单，三个外卖大佬里，饿了么的色调和布局是最漂亮的，看起来最舒服。

此项目大大小小共 45 个页面，涉及注册、登录、商品展示、购物车、下单等等，是一个完整的流程。一般公司即便是官网的单页面项目都没这么复杂，如果这个项目能驾驭的了，相信大部分公司的其他单页面应用也就不在话下，即便更复杂，也不会比这个高到哪里去。

因为利用业余时间来做，年前就开始写，又跨个年，周期有点长，项目从零布局到完成共用了2个多月的时间，目前项目已经完成，正在进行一些性能的优化，增加详细的注释。

另外，这个项目和慕课网视频的那个饿了么没有任何关系，慕课网的项目只有一个页面，我在看完vue的官方文档后直接写了这个项目，没有参照任何人的代码，请大家不要混为一谈。

__注：此项目纯属个人瞎搞，正常下单请选择饿了么官方客户端。__




## 技术栈
vue2 + vuex + vue-router + webpack + ES6/7 + fetch + sass + flex + svg



# 项目运行

#### 注意：由于涉及大量的 ES6/7 等新属性，nodejs 必须是 6.0 以上版本 ，node 7 是先行版，有可能会出问题，建议使用 node 6 稳定版

```
git clone https://github.com/bailicangdu/vue2-elm.git  

cd vue2-elm

npm install

```

### 编译环境
```
npm run dev

访问 http://localhost:8088
```


### 线上版本
```
npm run build

生成的elm文件夹放在服务器即可正常访问
```




# 说明

>  本项目主要用于熟悉如何用 vue2 架构一个大型项目

>  如果对您有帮助，您可以点右上角 "Star" 支持一下 谢谢！ ^_^

>  或者您可以 "follow" 一下，我会不断开源更多的有趣的项目

>  开发环境 macOS 10.12.3  Chrome 55

>  特别感谢辰妹子，在百忙之中抽出时间和我一起完成了这个项目，辛苦了🌹

>  如有问题请直接在 Issues 中提，或者您发现问题并有非常好的解决方案，欢迎 PR 👍

>  推荐一个 react + redux 开源项目，对react感兴趣的朋友赶紧去看看。[地址在这里](https://github.com/bailicangdu/react-pxq)

>  另外一个 vue2 + vuex 的入门项目，比当前的项目简单很多，非常适合入门练习。[地址在这里](https://github.com/bailicangdu/vue2-happyfri)



# 关于 demo 与 数据 的说明🤔

1、下载代码运行后，因为开启了反向代理，可以获取真实的官方数据，最终可以进行下单(真实的下单，而不是模拟，下单后可以在官方App中查看并付款，亲自试过，且成功付款点餐)，但是为了安全起见，登录的帐号为固定的帐号，以免泄露个人信息，不过照样可以点餐。

2、demo的数据为模拟的固定数据，只做为效果演示，因为反向代理必须在PC端运行代码才行。


## 效果演示

#### (demo使用的是模拟数据，数据是固定的，只做为样式的演示，要获取真实的数据，请clone代码并运行);

[查看demo请戳这里](http://test.fe.ptdev.cn/elm/)（请用chrome手机模式预览）

### 移动端扫描下方二维码

![](https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/elm_ewm.png)





# 目标功能
- [x] 定位功能 -- 完成
- [x] 选择城市 -- 完成
- [x] 搜索地址 -- 完成
- [x] 展示所选地址附近商家列表 -- 完成
- [x] 搜索美食，餐馆 -- 完成
- [x] 根据距离、销量、评分、特色菜、配送方式等进行排序和筛选 -- 完成
- [x] 餐馆食品列表页 -- 完成
- [x] 购物车功能 -- 完成
- [x] 店铺评价页面 -- 完成
- [x] 单个食品详情页面 -- 完成
- [x] 商家详情页 -- 完成
- [x] 登录、注册 -- 完成
- [x] 修改密码 -- 完成
- [x] 个人中心 -- 完成
- [x] 发送短信、语音验证 -- 完成
- [x] 下单功能 -- 完成 ✨✨🎉🎉
- [x] 订单列表 -- 完成
- [x] 订单详情 -- 完成
- [x] 下载App -- 完成
- [x] 添加、删除、修改收货地址 -- 完成
- [x] 帐户信息 -- 完成
- [x] 服务中心 -- 完成
- [x] 红包 -- 完成
- [x] 上传头像 -- 完成
- [ ] 付款 -- 臣妾做不到啊~~



# 总结

1、因为并不是elm官方，而且因为要开代理，必须在pc端打开，最多只能做到下单这一步，下单成功后可以在手机客户端查看并付款。

2、一般涉及到money的网页逻辑都比较复杂，尤其像饿了么这样一个开放的平台，商家和食品种类繁多，页面与页面之间交互复杂，在写到 购物车 和 下单 功能时众多的数据和逻辑一度让人很头疼，又没有设计和接口api文档，只能一步步摸索。

3、vue因其轻量级的框架在中小型项目中表现亮眼，在大型单页面应用中因为vuex的存在，表现依然出色，在处理复杂交互逻辑的时候，vuex的存在是不可或缺的。所以说利用 vue + vuex 完全可以去做大型的单页面项目。

4、项目写到现在，从 登录注册到、首页、搜索、商家列表、购物车、下单、订单列表、个人中心 一个流程走完之后、不但对vue的理解更深一层，而且对以后掌控大型项目的时候也有非常多的帮助，做一个实际的项目才能对自己有很大的提升。

5、曾一度怀疑，花几个月的时间做这样一个项目到底有没有意义，本来只是想做一个小项目练练手，没想到后来越写越多，不过坚持下来后我相信一切都是值得的。

6、项目已经完成，共45个页面。


# 最终目标

1、用node.js构建一个模拟外卖平台的后台系统。(已经开始制作)

2、利用 react-native 写出跨 Android 和 IOS 的原生APP版本。

3、如果时间来的及，会出一个pc端的网页版。

所以我的目的是构建一个横跨前后端，移动IOS、Android的完整生态圈。

。。。敬请期待




# 部分截图


### 商铺列表页

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/msite.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/msite.gif" width="365" height="619"/>


### 商铺筛选页

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/food.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/food.gif" width="365" height="619"/>



### 餐馆食品列表与购物车

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/shop_cart.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/shop_cart.gif" width="365" height="619"/>

### 确认订单页

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/confirm1.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/confirmOrder.gif" width="365" height="619"/>


### 搜索页

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/search.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/search.gif" width="365" height="619"/>


### 登录页

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/login1.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/login.gif" width="365" height="619"/>


### 个人中心

<img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/profile.png" width="365" height="619"/> <img src="https://github.com/bailicangdu/vue2-elm/blob/master/screenshots/profile.gif" width="365" height="619"/>






# 项目布局

```
.
├── build										// webpack配置文件
├── config										// 项目打包路径
├── elm											// 上线项目文件，放在服务器即可正常访问
├── screenshots									// 项目截图
├── src											// 源码目录
│   ├── App.vue
│   ├── components
│   │   ├── common
│   │   │   ├── alertTip.vue
│   │   │   ├── buyCart.vue
│   │   │   ├── computeTime.vue
│   │   │   ├── loading.vue
│   │   │   ├── mixin.js
│   │   │   ├── ratingStar.vue
│   │   │   └── shoplist.vue
│   │   ├── footer
│   │   │   └── footGuide.vue
│   │   └── header
│   │       └── head.vue
│   ├── config
│   │   ├── env.js
│   │   ├── fetch.js
│   │   ├── mUtils.js
│   │   └── rem.js
│   ├── images
│   ├── main.js
│   ├── page
│   │   ├── balance
│   │   │   ├── balance.vue
│   │   │   └── children
│   │   │       └── detail.vue
│   │   ├── benefit
│   │   │   ├── benefit.vue
│   │   │   └── children
│   │   │       ├── commend.vue
│   │   │       ├── coupon.vue
│   │   │       ├── exchange.vue
│   │   │       ├── hbDescription.vue
│   │   │       └── hbHistory.vue
│   │   ├── city
│   │   │   └── city.vue
│   │   ├── confirmOrder
│   │   │   ├── children
│   │   │   │   ├── children
│   │   │   │   │   ├── addAddress.vue
│   │   │   │   │   └── children
│   │   │   │   │       └── searchAddress.vue
│   │   │   │   ├── chooseAddress.vue
│   │   │   │   ├── invoice.vue
│   │   │   │   ├── payment.vue
│   │   │   │   ├── remark.vue
│   │   │   │   └── userValidation.vue
│   │   │   └── confirmOrder.vue
│   │   ├── download
│   │   │   └── download.vue
│   │   ├── find
│   │   │   └── find.vue
│   │   ├── food
│   │   │   └── food.vue
│   │   ├── forget
│   │   │   └── forget.vue
│   │   ├── home
│   │   │   └── home.vue
│   │   ├── login
│   │   │   └── login.vue
│   │   ├── msite
│   │   │   └── msite.vue
│   │   ├── order
│   │   │   ├── children
│   │   │   │   └── orderDetail.vue
│   │   │   └── order.vue
│   │   ├── points
│   │   │   ├── children
│   │   │   │   └── detail.vue
│   │   │   └── points.vue
│   │   ├── profile
│   │   │   ├── children
│   │   │   │   ├── children
│   │   │   │   │   ├── address.vue
│   │   │   │   │   └── children
│   │   │   │   │       ├── add.vue
│   │   │   │   │       └── children
│   │   │   │   │           └── addDetail.vue
│   │   │   │   ├── info.vue
│   │   │   │   └── setusername.vue
│   │   │   └── profile.vue
│   │   ├── search
│   │   │   └── search.vue
│   │   ├── service
│   │   │   ├── children
│   │   │   │   └── questionDetail.vue
│   │   │   └── service.vue
│   │   ├── shop
│   │   │   ├── children
│   │   │   │   ├── children
│   │   │   │   │   └── shopSafe.vue
│   │   │   │   ├── foodDetail.vue
│   │   │   │   └── shopDetail.vue
│   │   │   └── shop.vue
│   │   └── vipcard
│   │       ├── children
│   │       │   ├── invoiceRecord.vue
│   │       │   ├── useCart.vue
│   │       │   └── vipDescription.vue
│   │       └── vipcard.vue
│   ├── plugins
│   │   └── swiper.min.js
│   ├── router
│   │   └── router.js
│   ├── service
│   │   ├── getData.js
│   │   └── tempdata
│   ├── store
│   │   ├── action.js
│   │   ├── getters.js
│   │   ├── index.js
│   │   ├── modules
│   │   ├── mutation-types.js
│   │   └── mutations.js
│   └── style
│       ├── common.scss
│       ├── mixin.scss
│       └── swiper.min.css
├── favicon.ico
├── index.html

56 directories, 203 files
```