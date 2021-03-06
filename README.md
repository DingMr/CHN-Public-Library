# China Public Library

## Info

### 宗旨

本 Repo 旨在收集整理国内城市公益性图书馆（包括非公益性机构的免费开放区域）信息，侧重图书馆提供的自修（习）及相应服务，不涉及馆藏书籍等信息。因为（个人认为）现代书籍已趋向数字化，图书馆作为物理空间应该提供更多的城市公共服务（ LaaS, Library as a Service )。信息主要由个人收集整理，相应参数评级均有本人亲临现场确认评分，具有极强主观性，参考价值请自行考量。

由于本人居住于成都，如有其它城市的小伙伴 PR 自己的城市十分欢迎，但请确保至少本人去过一次。参数设计合理性也欢迎提 Issue 探讨。

### 城市

- [成都 (15)](./chengdu.geojson)
- [广州 (1)](./guangzhou.geojson)

### 评分简述

| 参数名称 | 参数类型 |                             分值说明                             |
| :------: | :------: | :--------------------------------------------------------------: |
|   名称   |  String  |                                                                  |
|   级别   |  String  |        1-社区街道级；2-区县级；3-市级；4-省级；5-国家级；        |
| 开放时间 |  String  |                         星期：开闭馆时间                         |
|   新旧   |  Number  |    装饰及设备新旧程度：1-陈旧;2-较旧；3-中等；4-较新；5-崭新     |
|   体量   |  Number  |    占地面积及建筑体量：1-微缩；2-较小；3-中等；4-较大；5-宏伟    |
|   座位   |  Number  |      提供自修座位量：1-稀缺；2-较少；3-中等；4-较多；5-充沛      |
|  光环境  |  Number  |       室内光照环境：1-昏暗；2-较暗；3-中等；4-较亮；5-明亮       |
|  声环境  |  Number  |       室内安静程度：1-嘈杂；2-较吵；3-中等；4-较静；5-安静       |
|  热环境  |  Number  |       室内制冷供热：1-恶劣；2-较差；3-中等；4-较好；5-舒适       |
| 热水供应 | Boolean  |           馆内是否免费提供可饮热水：true-是；false-否            |
| 凉水供应 | Boolean  |          馆内是否免费提供可直饮凉水：true-是；false-否           |
| 用餐区域 | Boolean  |             馆内是否提供用餐区域：true-是；false-否              |
| 电源插座 | Boolean  |              座位上是否提供插座：true-是；false-否               |
| 网络质量 |  Number  | 无线网速率及稳定性：0-无；1-摆设；2-较差；3-中等；4-较好；5-极好 |

- 数值型参数均为 5 分制，数值越大表示越优；
- 若参数值为 null 表示未知；
- 图书馆分级参考大体对应行政等级，旨在尽量匹配图书馆规模，提供一个大致的直观印感受（[未使用国家公共图书馆分级是因为实际意义不大](http://www.lsc.org.cn/contents/1129/12564.html#)），但这个对应关系不总是成立，比如有些区县级图书馆的规模比市级还大；
- 市级图书馆分馆归类到县区级，区县级图书馆分馆归类到社区、街道图书馆；
- 高校图书馆仅添加对外开放的，暂且粗略地归类至县区级；
- Wi-Fi 速率测试尽量避免选择城市公共热点（如 i-chengdu ）进行，而是优先选择图书馆自行提供的 Wi-Fi 服务。

### 样式

|    等级    | 图标大小 | 图标颜色 |
| :--------: | :------: | :------: |
|   国家级   |  large   | \#FF0000 |
|    省级    |  large   | \#CC6633 |
|    市级    |  medium  | \#339900 |
|   区县级   |  medium  | \#0099FF |
| 社区街道级 |  small   | \#333333 |

## Todo

- [ ] 系统： - [x] 增加分类图标 - [x] 完善图书馆级别体系 - [ ] CI integrate - [ ] i18n - [ ] 主页，提供更便捷的查看

- [ ] 成都：

  - [ ] 补全二绕内区县级图书馆
  - [ ] 增加部分社区级图书馆（包括城市阅读空间）
  - [ ] 增加对外开放的高校图书馆

## Thanks

该 Repo 灵感源于 [cn-cafe](https://github.com/ElaWorkshop/awesome-cn-cafe) ，在此以表谢意。
