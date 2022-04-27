[![](https://img.shields.io/badge/EpidemicStatisticsTable-@Vogadero-success.svg?style=plastic)](https://github.com/Vogadero/EpidemicStatisticsTable)
![](https://img.shields.io/badge/language-Jquery-yellow.svg?style=plastic)
![](https://img.shields.io/badge/language-JavaScript-orange.svg?style=plastic)
![](https://img.shields.io/badge/language-Html-9cf.svg?style=plastic)
![](https://img.shields.io/badge/language-Css-blueviolet.svg?style=plastic)
![](https://img.shields.io/npm/l/express?style=plastic)

# 项目简介🚩

- 疫情统计表
- 演示地址：https://vogadero.github.io/EpidemicStatisticsTable/

## 1. 功能模块🎨

#### 1.1 首页🛫

| 功能         |
| ------------ |
| 展示统计列表 |

## 2. 截图⭐

![](images/01.jpeg)

## 3. 项目架构🍽️

| 系统分层 | 使用技术             |
| -------- | -------------------- |
| 客户端   | art-template、jQuery |

## 4. 项目运行环境搭建🌈

- 克隆远端数据仓库到本地：`git clone 仓库地址`
- 拉取远程仓库中最新的版本：`git pull 远程仓库地址 分支名称`
- 双击index.html

# 功能介绍🦷

## 🕵️‍♀️标题

- 展示内容：昨日本土新增、境外输入、港澳台病例数

- API

  - 地址：https://view.inews.qq.com/g2/getOnsInfo

  - 方式：GET

  - 参数类型：jsonp

  - 参数：

    | 参数名 | 说明                     |
    | ------ | ------------------------ |
    | name   | wuwei_ww_ww_today_notice |

    

## :card_index:**中国疫情总概**

- 展示内容：本土现有确诊(不含港澳台、不含境外输入)；现有确诊(含港澳台)；累计确诊；无症状感染者；境外输入；累计死亡以及较上日数据情况变化

- API

  - 地址：https://api.inews.qq.com/newsqa/v1/query/inner/publish/modules/list

  - 方式：GET

  - 参数：

    | 参数名  | 说明                                 |
    | ------- | ------------------------------------ |
    | modules | statisGradeCityDetail,diseaseh5Shelf |

    

  

## :woman_technologist:**国内外新冠疫苗接种追踪**

- 展示内容：国内外累计接种数；较上日新增数；每百人接种数

- API

  - 地址：https://api.inews.qq.com/newsqa/v1/automation/modules/list

  - 方式：GET

  - 参数：

    | 参数名  | 说明           |
    | ------- | -------------- |
    | modules | VaccineTopData |

    



## :thermometer:**近期31省区市本土病例**

- 展示内容：近期31省区市本土新增、现有确诊、累计确诊、治愈以及死亡数据情况

- API

  - 地址：https://api.inews.qq.com/newsqa/v1/query/inner/publish/modules/list

  - 方式：GET

  - 参数：

    | 参数名  | 说明                                 |
    | ------- | ------------------------------------ |
    | modules | statisGradeCityDetail,diseaseh5Shelf |



## :four_leaf_clover:**风险地区统计**

- 展示内容：31省中高风险地区统计，其中标红为高风险地区
- API
  - 地址：https://eyesight.news.qq.com/sars/riskarea
  - 方式：GET
  - 参数类型：jsonp



# Tree🌵    


```
疫情统计表
├─ assets	// bootstrap框架
│  └─ bootstrap
│     ├─ CHANGELOG.md
│     ├─ dist
│     │  ├─ css
│     │  │  ├─ bootstrap-theme.css
│     │  │  ├─ bootstrap-theme.css.map
│     │  │  ├─ bootstrap-theme.min.css
│     │  │  ├─ bootstrap-theme.min.css.map
│     │  │  ├─ bootstrap.css
│     │  │  ├─ bootstrap.css.map
│     │  │  ├─ bootstrap.min.css
│     │  │  └─ bootstrap.min.css.map
│     │  ├─ fonts
│     │  │  ├─ glyphicons-halflings-regular.eot
│     │  │  ├─ glyphicons-halflings-regular.svg
│     │  │  ├─ glyphicons-halflings-regular.ttf
│     │  │  ├─ glyphicons-halflings-regular.woff
│     │  │  └─ glyphicons-halflings-regular.woff2
│     │  └─ js
│     │     ├─ bootstrap.js
│     │     ├─ bootstrap.min.js
│     │     └─ npm.js
│     ├─ fonts
│     │  ├─ glyphicons-halflings-regular.eot
│     │  ├─ glyphicons-halflings-regular.svg
│     │  ├─ glyphicons-halflings-regular.ttf
│     │  ├─ glyphicons-halflings-regular.woff
│     │  └─ glyphicons-halflings-regular.woff2
│     ├─ grunt
│     │  ├─ .jshintrc
│     │  ├─ bs-commonjs-generator.js
│     │  ├─ bs-glyphicons-data-generator.js
│     │  ├─ bs-lessdoc-parser.js
│     │  ├─ bs-raw-files-generator.js
│     │  ├─ change-version.js
│     │  ├─ configBridge.json
│     │  ├─ npm-shrinkwrap.json
│     │  └─ sauce_browsers.yml
│     ├─ Gruntfile.js
│     ├─ js
│     │  ├─ affix.js
│     │  ├─ alert(1).js
│     │  ├─ button.js
│     │  ├─ carousel.js
│     │  ├─ collapse.js
│     │  ├─ dropdown.js
│     │  ├─ modal.js
│     │  ├─ popover.js
│     │  ├─ scrollspy.js
│     │  ├─ tab.js
│     │  ├─ tooltip.js
│     │  └─ transition.js
│     ├─ less
│     │  ├─ alerts.less
│     │  ├─ badges.less
│     │  ├─ bootstrap.less
│     │  ├─ breadcrumbs.less
│     │  ├─ button-groups.less
│     │  ├─ buttons.less
│     │  ├─ carousel.less
│     │  ├─ close.less
│     │  ├─ code.less
│     │  ├─ component-animations.less
│     │  ├─ dropdowns.less
│     │  ├─ forms.less
│     │  ├─ glyphicons.less
│     │  ├─ grid.less
│     │  ├─ input-groups.less
│     │  ├─ jumbotron.less
│     │  ├─ labels.less
│     │  ├─ list-group.less
│     │  ├─ media.less
│     │  ├─ mixins
│     │  │  ├─ alerts.less
│     │  │  ├─ background-variant.less
│     │  │  ├─ border-radius.less
│     │  │  ├─ buttons.less
│     │  │  ├─ center-block.less
│     │  │  ├─ clearfix.less
│     │  │  ├─ forms.less
│     │  │  ├─ gradients.less
│     │  │  ├─ grid-framework.less
│     │  │  ├─ grid.less
│     │  │  ├─ hide-text.less
│     │  │  ├─ image.less
│     │  │  ├─ labels.less
│     │  │  ├─ list-group.less
│     │  │  ├─ nav-divider.less
│     │  │  ├─ nav-vertical-align.less
│     │  │  ├─ opacity.less
│     │  │  ├─ pagination.less
│     │  │  ├─ panels.less
│     │  │  ├─ progress-bar.less
│     │  │  ├─ reset-filter.less
│     │  │  ├─ reset-text.less
│     │  │  ├─ resize.less
│     │  │  ├─ responsive-visibility.less
│     │  │  ├─ size.less
│     │  │  ├─ tab-focus.less
│     │  │  ├─ table-row.less
│     │  │  ├─ text-emphasis.less
│     │  │  ├─ text-overflow.less
│     │  │  └─ vendor-prefixes.less
│     │  ├─ mixins.less
│     │  ├─ modals.less
│     │  ├─ navbar.less
│     │  ├─ navs.less
│     │  ├─ normalize.less
│     │  ├─ pager.less
│     │  ├─ pagination.less
│     │  ├─ panels.less
│     │  ├─ popovers.less
│     │  ├─ print.less
│     │  ├─ progress-bars.less
│     │  ├─ responsive-embed.less
│     │  ├─ responsive-utilities.less
│     │  ├─ scaffolding.less
│     │  ├─ tables.less
│     │  ├─ theme.less
│     │  ├─ thumbnails.less
│     │  ├─ tooltip.less
│     │  ├─ type.less
│     │  ├─ utilities.less
│     │  ├─ variables.less
│     │  └─ wells.less
│     ├─ LICENSE
│     ├─ package.json
│     └─ README.md
├─ images	// 项目截图和logo
│  ├─ 01.jpeg
│  └─ favicon.ico
├─ index.html	// 首页
├─ js	// 脚本
│  ├─ jquery.js
│  └─ template-web.js
└─ README.md
```
