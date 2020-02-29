
## 1.介绍说明

本项目是使用[diseasedataarrange](https://github.com/zyq5945/diseasedataarrange)程序，针对[DXY-COVID-19-Data](https://github.com/BlankerL/DXY-COVID-19-Data)的最新DXYArea.csv文件，自动生成整理后的数组JSON格式文件数据。

若你对生成的数据有疑问,或者认为汇总的数据有误，请向[BlankerL反馈异常数据](https://github.com/BlankerL/DXY-COVID-19-Crawler/issues/34)

## 2.不同平台访问地址

针对可能对不同网站访问速度有快慢问题，酌情可以考虑以下最快的访问地址：

### [github.com 仓库地址](https://github.com/zyq5945/DXY-COVID-19-Data-Arrange-AJSON)

### [github.io  网页地址](https://zyq5945.github.com/DXY-COVID-19-Data-Arrange-AJSON)


## 3.生成文件的说明

### 3.1 文件目录说明

| 目录名 |  说明 |
|---|---|
|  ChildDetail | 各个子按日期升序排序的详细情况目录，其下是各父名称目录，父目录下才是子文件 |
|  ParentDetail | 各个父按日期升序排序的详细情况目录 |
|  ParentLastChildren | 各个子按日期降序排序的最后更新情况目录，其下是各父名称目录，父目录下才是子文件 |


### 3.2 固定文件名称说明

| 文件名 |  说明 |
|---|---|
|  Total | 最后更新汇总的情况 |
|  LastParents | 最后更新的所有父情况 |
|  LastChildren | 最后更新的所有子情况 |


### 3.3 文件的各字段说明

注：标准化是指将值缩放到浮点数是0-1之间的值

| 字段 |  说明 |
|---|---|
|  TimeOffset | 浮点型的天数时间偏移 |
|  UpdateTime | 更新时间 |
|  ParentName | 父名称 |
|  ParentConfirmedCount | 父确诊数 |
|  ParentSuspectedCount | 父疑似数 |
|  ParentCuredCount | 父康复数 |
|  ParentDeadCount | 父死亡数 |
|  ParentTreatingCount | 父正在治疗数 |
|  ParentCuredRate | 父康复率 |
|  ParentDeadRate | 父死亡率 |
|  ParentTreatingRate | 父正在治疗率 |
|  ParentDeadDivideCured | 父死亡除以康复数 |
|  ParentCuredDivideDead | 父康复除以死亡数 |
|  ParentConfirmedNorm | 父确诊数标准化 |
|  ParentSuspectedNorm | 父疑似数标准化 |
|  ParentCuredNorm | 父康复数标准化 |
|  ParentDeadNorm | 父死亡数标准化 |
|  ParentTreatingNorm | 父正在治疗数标准化 |
|  ParentDeadDivideCuredNorm | 父确诊数标准化 |
|  ParentCuredDivideDeadNorm | 父康复除以死亡数标准化 |
|  ParentTatalConfirmedNorm | 总计的父确诊数标准化 |
|  ParentTatalSuspectedNorm | 总计的父疑似数标准化 |
|  ParentTatalCuredNorm | 总计的父康复数标准化 |
|  ParentTatalDeadNorm | 总计的父死亡数标准化 |
|  ParentTatalTreatingNorm | 总计的父正在治疗数标准化 |
|  ChildName | 子名称 |
|  ChildConfirmedCount | 子确诊数 |
|  ChildSuspectedCount | 子疑似数 |
|  ChildCuredCount | 子康复数 |
|  ChildDeadCount | 子死亡数 |
|  ChildTreatingCount | 子正在治疗数 |
|  ChildCuredRate | 子康复率 |
|  ChildDeadRate | 子死亡率 |
|  ChildTreatingRate | 子正在治疗率 |
|  ChildDeadDivideCured | 子死亡除以康复数 |
|  ChildCuredDivideDead | 子康复除以死亡数 |
|  ChildConfirmedCountRate | 子确诊数相对父占比率 |
|  ChildSuspectedCountRate | 子疑似数相对父占比率 |
|  ChildCuredCountRate | 子确康复数相对父占比率 |
|  ChildDeadCountRate | 子确死亡数相对父占比率 |
|  ChildTreatingCountRate | 子正在治疗数相对父占比率 |
|  ChildConfirmedNorm | 子确诊数标准化 |
|  ChildSuspectedNorm | 子疑似数标准化 |
|  ChildCuredNorm | 子康复数标准化 |
|  ChildDeadNorm | 子死亡数标准化 |
|  ChildTreatingNorm | 子正在治疗数标准化 |
|  ChildDeadDivideCuredNorm | 子确诊数标准化 |
|  ChildCuredDivideDeadNorm | 子康复除以死亡数标准化 |
|  ChildTatalConfirmedNorm | 总计的子确诊数标准化 |
|  ChildTatalSuspectedNorm | 总计的子疑似数标准化 |
|  ChildTatalCuredNorm | 总计的子康复数标准化 |
|  ChildTatalDeadNorm | 总计的子死亡数标准化 |
|  ChildTatalTreatingNorm | 总计的子正在治疗数标准化 |

## 4.生成的文件查看地址

### 4.1 汇总文件

|名称|
|---|
|[Total](./data/Total.json)|
|[LastParents](./data/LastParents.json)|
|[LastChildren](./data/LastChildren.json)|


### 4.2 各个父按日期升序排序的详细情况目录

|名称|
|---|
|[安徽](./data/ParentDetail/安徽.json)|
|[澳门](./data/ParentDetail/澳门.json)|
|[北京](./data/ParentDetail/北京.json)|
|[福建](./data/ParentDetail/福建.json)|
|[甘肃](./data/ParentDetail/甘肃.json)|
|[广东](./data/ParentDetail/广东.json)|
|[广西](./data/ParentDetail/广西.json)|
|[贵州](./data/ParentDetail/贵州.json)|
|[海南](./data/ParentDetail/海南.json)|
|[河北](./data/ParentDetail/河北.json)|
|[河南](./data/ParentDetail/河南.json)|
|[黑龙江](./data/ParentDetail/黑龙江.json)|
|[湖北](./data/ParentDetail/湖北.json)|
|[湖南](./data/ParentDetail/湖南.json)|
|[吉林](./data/ParentDetail/吉林.json)|
|[江苏](./data/ParentDetail/江苏.json)|
|[江西](./data/ParentDetail/江西.json)|
|[辽宁](./data/ParentDetail/辽宁.json)|
|[内蒙古](./data/ParentDetail/内蒙古.json)|
|[宁夏](./data/ParentDetail/宁夏.json)|
|[青海](./data/ParentDetail/青海.json)|
|[山东](./data/ParentDetail/山东.json)|
|[山西](./data/ParentDetail/山西.json)|
|[陕西](./data/ParentDetail/陕西.json)|
|[上海](./data/ParentDetail/上海.json)|
|[四川](./data/ParentDetail/四川.json)|
|[天津](./data/ParentDetail/天津.json)|
|[西藏](./data/ParentDetail/西藏.json)|
|[新疆](./data/ParentDetail/新疆.json)|
|[云南](./data/ParentDetail/云南.json)|
|[浙江](./data/ParentDetail/浙江.json)|
|[重庆](./data/ParentDetail/重庆.json)|

### 4.3 各个子按日期降序排序的最后更新情况目录

|名称|
|---|
|[安徽](./data/ParentLastChildren/安徽.json)|
|[澳门](./data/ParentLastChildren/澳门.json)|
|[北京](./data/ParentLastChildren/北京.json)|
|[福建](./data/ParentLastChildren/福建.json)|
|[甘肃](./data/ParentLastChildren/甘肃.json)|
|[广东](./data/ParentLastChildren/广东.json)|
|[广西](./data/ParentLastChildren/广西.json)|
|[贵州](./data/ParentLastChildren/贵州.json)|
|[海南](./data/ParentLastChildren/海南.json)|
|[河北](./data/ParentLastChildren/河北.json)|
|[河南](./data/ParentLastChildren/河南.json)|
|[黑龙江](./data/ParentLastChildren/黑龙江.json)|
|[湖北](./data/ParentLastChildren/湖北.json)|
|[湖南](./data/ParentLastChildren/湖南.json)|
|[吉林](./data/ParentLastChildren/吉林.json)|
|[江苏](./data/ParentLastChildren/江苏.json)|
|[江西](./data/ParentLastChildren/江西.json)|
|[辽宁](./data/ParentLastChildren/辽宁.json)|
|[内蒙古](./data/ParentLastChildren/内蒙古.json)|
|[宁夏](./data/ParentLastChildren/宁夏.json)|
|[青海](./data/ParentLastChildren/青海.json)|
|[山东](./data/ParentLastChildren/山东.json)|
|[山西](./data/ParentLastChildren/山西.json)|
|[陕西](./data/ParentLastChildren/陕西.json)|
|[上海](./data/ParentLastChildren/上海.json)|
|[四川](./data/ParentLastChildren/四川.json)|
|[天津](./data/ParentLastChildren/天津.json)|
|[西藏](./data/ParentLastChildren/西藏.json)|
|[新疆](./data/ParentLastChildren/新疆.json)|
|[云南](./data/ParentLastChildren/云南.json)|
|[浙江](./data/ParentLastChildren/浙江.json)|
|[重庆](./data/ParentLastChildren/重庆.json)|

### 4.4 各个子按日期升序排序的详细情况目录

|名称|
|---|
|[安徽_安庆](./data/ChildDetail/安徽/安庆.json)|
|[安徽_蚌埠](./data/ChildDetail/安徽/蚌埠.json)|
|[安徽_亳州](./data/ChildDetail/安徽/亳州.json)|
|[安徽_池州](./data/ChildDetail/安徽/池州.json)|
|[安徽_滁州](./data/ChildDetail/安徽/滁州.json)|
|[安徽_待明确地区](./data/ChildDetail/安徽/待明确地区.json)|
|[安徽_阜阳](./data/ChildDetail/安徽/阜阳.json)|
|[安徽_合肥](./data/ChildDetail/安徽/合肥.json)|
|[安徽_淮北](./data/ChildDetail/安徽/淮北.json)|
|[安徽_淮南](./data/ChildDetail/安徽/淮南.json)|
|[安徽_黄山](./data/ChildDetail/安徽/黄山.json)|
|[安徽_六安](./data/ChildDetail/安徽/六安.json)|
|[安徽_马鞍山](./data/ChildDetail/安徽/马鞍山.json)|
|[安徽_铜陵](./data/ChildDetail/安徽/铜陵.json)|
|[安徽_芜湖](./data/ChildDetail/安徽/芜湖.json)|
|[安徽_歙县](./data/ChildDetail/安徽/歙县.json)|
|[安徽_宿松](./data/ChildDetail/安徽/宿松.json)|
|[安徽_宿州](./data/ChildDetail/安徽/宿州.json)|
|[安徽_宣城](./data/ChildDetail/安徽/宣城.json)|
|[澳门_澳门](./data/ChildDetail/澳门/澳门.json)|
|[北京_昌平](./data/ChildDetail/北京/昌平.json)|
|[北京_朝阳](./data/ChildDetail/北京/朝阳.json)|
|[北京_大兴](./data/ChildDetail/北京/大兴.json)|
|[北京_待明确地区](./data/ChildDetail/北京/待明确地区.json)|
|[北京_东城](./data/ChildDetail/北京/东城.json)|
|[北京_房山](./data/ChildDetail/北京/房山.json)|
|[北京_丰台](./data/ChildDetail/北京/丰台.json)|
|[北京_海淀](./data/ChildDetail/北京/海淀.json)|
|[北京_怀柔](./data/ChildDetail/北京/怀柔.json)|
|[北京_门头沟](./data/ChildDetail/北京/门头沟.json)|
|[北京_密云](./data/ChildDetail/北京/密云.json)|
|[北京_石景山](./data/ChildDetail/北京/石景山.json)|
|[北京_顺义](./data/ChildDetail/北京/顺义.json)|
|[北京_通州](./data/ChildDetail/北京/通州.json)|
|[北京_外地来人员](./data/ChildDetail/北京/外地来人员.json)|
|[北京_西城](./data/ChildDetail/北京/西城.json)|
|[北京_延庆](./data/ChildDetail/北京/延庆.json)|
|[福建_待明确地区](./data/ChildDetail/福建/待明确地区.json)|
|[福建_福州](./data/ChildDetail/福建/福州.json)|
|[福建_龙岩](./data/ChildDetail/福建/龙岩.json)|
|[福建_南平](./data/ChildDetail/福建/南平.json)|
|[福建_宁德](./data/ChildDetail/福建/宁德.json)|
|[福建_莆田](./data/ChildDetail/福建/莆田.json)|
|[福建_泉州](./data/ChildDetail/福建/泉州.json)|
|[福建_三明](./data/ChildDetail/福建/三明.json)|
|[福建_厦门](./data/ChildDetail/福建/厦门.json)|
|[福建_漳州](./data/ChildDetail/福建/漳州.json)|
|[甘肃_白银](./data/ChildDetail/甘肃/白银.json)|
|[甘肃_待明确地区](./data/ChildDetail/甘肃/待明确地区.json)|
|[甘肃_定西](./data/ChildDetail/甘肃/定西.json)|
|[甘肃_甘南](./data/ChildDetail/甘肃/甘南.json)|
|[甘肃_金昌](./data/ChildDetail/甘肃/金昌.json)|
|[甘肃_兰州](./data/ChildDetail/甘肃/兰州.json)|
|[甘肃_临夏](./data/ChildDetail/甘肃/临夏.json)|
|[甘肃_陇南](./data/ChildDetail/甘肃/陇南.json)|
|[甘肃_平凉](./data/ChildDetail/甘肃/平凉.json)|
|[甘肃_庆阳](./data/ChildDetail/甘肃/庆阳.json)|
|[甘肃_天水](./data/ChildDetail/甘肃/天水.json)|
|[甘肃_张掖](./data/ChildDetail/甘肃/张掖.json)|
|[广东_潮州](./data/ChildDetail/广东/潮州.json)|
|[广东_待明确地区](./data/ChildDetail/广东/待明确地区.json)|
|[广东_东莞](./data/ChildDetail/广东/东莞.json)|
|[广东_佛山](./data/ChildDetail/广东/佛山.json)|
|[广东_广州](./data/ChildDetail/广东/广州.json)|
|[广东_河源](./data/ChildDetail/广东/河源.json)|
|[广东_惠州](./data/ChildDetail/广东/惠州.json)|
|[广东_江门](./data/ChildDetail/广东/江门.json)|
|[广东_揭阳](./data/ChildDetail/广东/揭阳.json)|
|[广东_茂名](./data/ChildDetail/广东/茂名.json)|
|[广东_梅州](./data/ChildDetail/广东/梅州.json)|
|[广东_清远](./data/ChildDetail/广东/清远.json)|
|[广东_汕头](./data/ChildDetail/广东/汕头.json)|
|[广东_汕尾](./data/ChildDetail/广东/汕尾.json)|
|[广东_韶关](./data/ChildDetail/广东/韶关.json)|
|[广东_深圳](./data/ChildDetail/广东/深圳.json)|
|[广东_外地来人员](./data/ChildDetail/广东/外地来人员.json)|
|[广东_阳江](./data/ChildDetail/广东/阳江.json)|
|[广东_湛江](./data/ChildDetail/广东/湛江.json)|
|[广东_肇庆](./data/ChildDetail/广东/肇庆.json)|
|[广东_中山](./data/ChildDetail/广东/中山.json)|
|[广东_珠海](./data/ChildDetail/广东/珠海.json)|
|[广西_百色](./data/ChildDetail/广西/百色.json)|
|[广西_北海](./data/ChildDetail/广西/北海.json)|
|[广西_待明确地区](./data/ChildDetail/广西/待明确地区.json)|
|[广西_防城港](./data/ChildDetail/广西/防城港.json)|
|[广西_贵港](./data/ChildDetail/广西/贵港.json)|
|[广西_桂林](./data/ChildDetail/广西/桂林.json)|
|[广西_河池](./data/ChildDetail/广西/河池.json)|
|[广西_贺州](./data/ChildDetail/广西/贺州.json)|
|[广西_来宾](./data/ChildDetail/广西/来宾.json)|
|[广西_柳州](./data/ChildDetail/广西/柳州.json)|
|[广西_南宁](./data/ChildDetail/广西/南宁.json)|
|[广西_钦州](./data/ChildDetail/广西/钦州.json)|
|[广西_梧州](./data/ChildDetail/广西/梧州.json)|
|[广西_玉林](./data/ChildDetail/广西/玉林.json)|
|[贵州_安顺](./data/ChildDetail/贵州/安顺.json)|
|[贵州_毕节](./data/ChildDetail/贵州/毕节.json)|
|[贵州_待明确地区](./data/ChildDetail/贵州/待明确地区.json)|
|[贵州_贵阳](./data/ChildDetail/贵州/贵阳.json)|
|[贵州_六盘水](./data/ChildDetail/贵州/六盘水.json)|
|[贵州_黔东南](./data/ChildDetail/贵州/黔东南.json)|
|[贵州_黔南](./data/ChildDetail/贵州/黔南.json)|
|[贵州_黔西南](./data/ChildDetail/贵州/黔西南.json)|
|[贵州_铜仁](./data/ChildDetail/贵州/铜仁.json)|
|[贵州_遵义](./data/ChildDetail/贵州/遵义.json)|
|[海南_保亭](./data/ChildDetail/海南/保亭.json)|
|[海南_昌江](./data/ChildDetail/海南/昌江.json)|
|[海南_澄迈](./data/ChildDetail/海南/澄迈.json)|
|[海南_待明确地区](./data/ChildDetail/海南/待明确地区.json)|
|[海南_儋州](./data/ChildDetail/海南/儋州.json)|
|[海南_定安](./data/ChildDetail/海南/定安.json)|
|[海南_东方](./data/ChildDetail/海南/东方.json)|
|[海南_海口](./data/ChildDetail/海南/海口.json)|
|[海南_乐东](./data/ChildDetail/海南/乐东.json)|
|[海南_临高](./data/ChildDetail/海南/临高.json)|
|[海南_陵水](./data/ChildDetail/海南/陵水.json)|
|[海南_琼海](./data/ChildDetail/海南/琼海.json)|
|[海南_琼中](./data/ChildDetail/海南/琼中.json)|
|[海南_三亚](./data/ChildDetail/海南/三亚.json)|
|[海南_万宁](./data/ChildDetail/海南/万宁.json)|
|[海南_文昌](./data/ChildDetail/海南/文昌.json)|
|[河北_保定](./data/ChildDetail/河北/保定.json)|
|[河北_沧州](./data/ChildDetail/河北/沧州.json)|
|[河北_承德](./data/ChildDetail/河北/承德.json)|
|[河北_邯郸](./data/ChildDetail/河北/邯郸.json)|
|[河北_衡水](./data/ChildDetail/河北/衡水.json)|
|[河北_廊坊](./data/ChildDetail/河北/廊坊.json)|
|[河北_秦皇岛](./data/ChildDetail/河北/秦皇岛.json)|
|[河北_石家庄](./data/ChildDetail/河北/石家庄.json)|
|[河北_唐山](./data/ChildDetail/河北/唐山.json)|
|[河北_邢台](./data/ChildDetail/河北/邢台.json)|
|[河北_张家口](./data/ChildDetail/河北/张家口.json)|
|[河南_安阳](./data/ChildDetail/河南/安阳.json)|
|[河南_待明确地区](./data/ChildDetail/河南/待明确地区.json)|
|[河南_邓州](./data/ChildDetail/河南/邓州.json)|
|[河南_巩义](./data/ChildDetail/河南/巩义.json)|
|[河南_固始](./data/ChildDetail/河南/固始.json)|
|[河南_鹤壁](./data/ChildDetail/河南/鹤壁.json)|
|[河南_滑县](./data/ChildDetail/河南/滑县.json)|
|[河南_济源](./data/ChildDetail/河南/济源.json)|
|[河南_焦作](./data/ChildDetail/河南/焦作.json)|
|[河南_开封](./data/ChildDetail/河南/开封.json)|
|[河南_洛阳](./data/ChildDetail/河南/洛阳.json)|
|[河南_漯河](./data/ChildDetail/河南/漯河.json)|
|[河南_南阳](./data/ChildDetail/河南/南阳.json)|
|[河南_平顶山](./data/ChildDetail/河南/平顶山.json)|
|[河南_濮阳](./data/ChildDetail/河南/濮阳.json)|
|[河南_三门峡](./data/ChildDetail/河南/三门峡.json)|
|[河南_商丘](./data/ChildDetail/河南/商丘.json)|
|[河南_新乡](./data/ChildDetail/河南/新乡.json)|
|[河南_信阳](./data/ChildDetail/河南/信阳.json)|
|[河南_许昌](./data/ChildDetail/河南/许昌.json)|
|[河南_永城](./data/ChildDetail/河南/永城.json)|
|[河南_长垣](./data/ChildDetail/河南/长垣.json)|
|[河南_郑州](./data/ChildDetail/河南/郑州.json)|
|[河南_周口](./data/ChildDetail/河南/周口.json)|
|[河南_驻马店](./data/ChildDetail/河南/驻马店.json)|
|[黑龙江_大庆](./data/ChildDetail/黑龙江/大庆.json)|
|[黑龙江_大兴安岭](./data/ChildDetail/黑龙江/大兴安岭.json)|
|[黑龙江_待明确地区](./data/ChildDetail/黑龙江/待明确地区.json)|
|[黑龙江_哈尔滨](./data/ChildDetail/黑龙江/哈尔滨.json)|
|[黑龙江_鹤岗](./data/ChildDetail/黑龙江/鹤岗.json)|
|[黑龙江_黑河](./data/ChildDetail/黑龙江/黑河.json)|
|[黑龙江_鸡西](./data/ChildDetail/黑龙江/鸡西.json)|
|[黑龙江_佳木斯](./data/ChildDetail/黑龙江/佳木斯.json)|
|[黑龙江_牡丹江](./data/ChildDetail/黑龙江/牡丹江.json)|
|[黑龙江_七台河](./data/ChildDetail/黑龙江/七台河.json)|
|[黑龙江_齐齐哈尔](./data/ChildDetail/黑龙江/齐齐哈尔.json)|
|[黑龙江_双鸭山](./data/ChildDetail/黑龙江/双鸭山.json)|
|[黑龙江_绥化](./data/ChildDetail/黑龙江/绥化.json)|
|[黑龙江_伊春](./data/ChildDetail/黑龙江/伊春.json)|
|[湖北_待明确地区](./data/ChildDetail/湖北/待明确地区.json)|
|[湖北_鄂州](./data/ChildDetail/湖北/鄂州.json)|
|[湖北_恩施](./data/ChildDetail/湖北/恩施.json)|
|[湖北_黄冈](./data/ChildDetail/湖北/黄冈.json)|
|[湖北_黄石](./data/ChildDetail/湖北/黄石.json)|
|[湖北_监狱系统](./data/ChildDetail/湖北/监狱系统.json)|
|[湖北_荆门](./data/ChildDetail/湖北/荆门.json)|
|[湖北_荆州](./data/ChildDetail/湖北/荆州.json)|
|[湖北_潜江](./data/ChildDetail/湖北/潜江.json)|
|[湖北_神农架林区](./data/ChildDetail/湖北/神农架林区.json)|
|[湖北_十堰](./data/ChildDetail/湖北/十堰.json)|
|[湖北_随州](./data/ChildDetail/湖北/随州.json)|
|[湖北_天门](./data/ChildDetail/湖北/天门.json)|
|[湖北_武汉](./data/ChildDetail/湖北/武汉.json)|
|[湖北_仙桃](./data/ChildDetail/湖北/仙桃.json)|
|[湖北_咸宁](./data/ChildDetail/湖北/咸宁.json)|
|[湖北_襄阳](./data/ChildDetail/湖北/襄阳.json)|
|[湖北_孝感](./data/ChildDetail/湖北/孝感.json)|
|[湖北_宜昌](./data/ChildDetail/湖北/宜昌.json)|
|[湖南_常德](./data/ChildDetail/湖南/常德.json)|
|[湖南_郴州](./data/ChildDetail/湖南/郴州.json)|
|[湖南_衡阳](./data/ChildDetail/湖南/衡阳.json)|
|[湖南_怀化](./data/ChildDetail/湖南/怀化.json)|
|[湖南_娄底](./data/ChildDetail/湖南/娄底.json)|
|[湖南_邵阳](./data/ChildDetail/湖南/邵阳.json)|
|[湖南_湘潭](./data/ChildDetail/湖南/湘潭.json)|
|[湖南_湘西](./data/ChildDetail/湖南/湘西.json)|
|[湖南_益阳](./data/ChildDetail/湖南/益阳.json)|
|[湖南_永州](./data/ChildDetail/湖南/永州.json)|
|[湖南_岳阳](./data/ChildDetail/湖南/岳阳.json)|
|[湖南_张家界](./data/ChildDetail/湖南/张家界.json)|
|[湖南_长沙](./data/ChildDetail/湖南/长沙.json)|
|[湖南_株洲](./data/ChildDetail/湖南/株洲.json)|
|[吉林_白城](./data/ChildDetail/吉林/白城.json)|
|[吉林_公主岭](./data/ChildDetail/吉林/公主岭.json)|
|[吉林_吉林](./data/ChildDetail/吉林/吉林.json)|
|[吉林_辽源](./data/ChildDetail/吉林/辽源.json)|
|[吉林_梅河口](./data/ChildDetail/吉林/梅河口.json)|
|[吉林_四平](./data/ChildDetail/吉林/四平.json)|
|[吉林_松原](./data/ChildDetail/吉林/松原.json)|
|[吉林_通化](./data/ChildDetail/吉林/通化.json)|
|[吉林_延边](./data/ChildDetail/吉林/延边.json)|
|[吉林_长春](./data/ChildDetail/吉林/长春.json)|
|[江苏_常州](./data/ChildDetail/江苏/常州.json)|
|[江苏_待明确地区](./data/ChildDetail/江苏/待明确地区.json)|
|[江苏_淮安](./data/ChildDetail/江苏/淮安.json)|
|[江苏_连云港](./data/ChildDetail/江苏/连云港.json)|
|[江苏_南京](./data/ChildDetail/江苏/南京.json)|
|[江苏_南通](./data/ChildDetail/江苏/南通.json)|
|[江苏_苏州](./data/ChildDetail/江苏/苏州.json)|
|[江苏_泰州](./data/ChildDetail/江苏/泰州.json)|
|[江苏_无锡](./data/ChildDetail/江苏/无锡.json)|
|[江苏_宿迁](./data/ChildDetail/江苏/宿迁.json)|
|[江苏_徐州](./data/ChildDetail/江苏/徐州.json)|
|[江苏_盐城](./data/ChildDetail/江苏/盐城.json)|
|[江苏_扬州](./data/ChildDetail/江苏/扬州.json)|
|[江苏_镇江](./data/ChildDetail/江苏/镇江.json)|
|[江西_待明确地区](./data/ChildDetail/江西/待明确地区.json)|
|[江西_抚州](./data/ChildDetail/江西/抚州.json)|
|[江西_赣江](./data/ChildDetail/江西/赣江.json)|
|[江西_赣州](./data/ChildDetail/江西/赣州.json)|
|[江西_吉安](./data/ChildDetail/江西/吉安.json)|
|[江西_景德镇](./data/ChildDetail/江西/景德镇.json)|
|[江西_九江](./data/ChildDetail/江西/九江.json)|
|[江西_南昌](./data/ChildDetail/江西/南昌.json)|
|[江西_萍乡](./data/ChildDetail/江西/萍乡.json)|
|[江西_上饶](./data/ChildDetail/江西/上饶.json)|
|[江西_新余](./data/ChildDetail/江西/新余.json)|
|[江西_宜春](./data/ChildDetail/江西/宜春.json)|
|[江西_鹰潭](./data/ChildDetail/江西/鹰潭.json)|
|[辽宁_鞍山](./data/ChildDetail/辽宁/鞍山.json)|
|[辽宁_本溪](./data/ChildDetail/辽宁/本溪.json)|
|[辽宁_朝阳](./data/ChildDetail/辽宁/朝阳.json)|
|[辽宁_大连](./data/ChildDetail/辽宁/大连.json)|
|[辽宁_待明确地区](./data/ChildDetail/辽宁/待明确地区.json)|
|[辽宁_丹东](./data/ChildDetail/辽宁/丹东.json)|
|[辽宁_阜新](./data/ChildDetail/辽宁/阜新.json)|
|[辽宁_葫芦岛](./data/ChildDetail/辽宁/葫芦岛.json)|
|[辽宁_锦州](./data/ChildDetail/辽宁/锦州.json)|
|[辽宁_辽阳](./data/ChildDetail/辽宁/辽阳.json)|
|[辽宁_盘锦](./data/ChildDetail/辽宁/盘锦.json)|
|[辽宁_沈阳](./data/ChildDetail/辽宁/沈阳.json)|
|[辽宁_铁岭](./data/ChildDetail/辽宁/铁岭.json)|
|[辽宁_营口](./data/ChildDetail/辽宁/营口.json)|
|[内蒙古_巴彦淖尔](./data/ChildDetail/内蒙古/巴彦淖尔.json)|
|[内蒙古_包头](./data/ChildDetail/内蒙古/包头.json)|
|[内蒙古_包头市东河](./data/ChildDetail/内蒙古/包头市东河.json)|
|[内蒙古_包头市昆都仑](./data/ChildDetail/内蒙古/包头市昆都仑.json)|
|[内蒙古_赤峰](./data/ChildDetail/内蒙古/赤峰.json)|
|[内蒙古_赤峰市林西县](./data/ChildDetail/内蒙古/赤峰市林西县.json)|
|[内蒙古_赤峰市松山区](./data/ChildDetail/内蒙古/赤峰市松山区.json)|
|[内蒙古_鄂尔多斯](./data/ChildDetail/内蒙古/鄂尔多斯.json)|
|[内蒙古_鄂尔多斯东胜](./data/ChildDetail/内蒙古/鄂尔多斯东胜.json)|
|[内蒙古_鄂尔多斯鄂托克前旗](./data/ChildDetail/内蒙古/鄂尔多斯鄂托克前旗.json)|
|[内蒙古_呼和浩特](./data/ChildDetail/内蒙古/呼和浩特.json)|
|[内蒙古_呼伦贝尔](./data/ChildDetail/内蒙古/呼伦贝尔.json)|
|[内蒙古_呼伦贝尔满洲里](./data/ChildDetail/内蒙古/呼伦贝尔满洲里.json)|
|[内蒙古_呼伦贝尔牙克石](./data/ChildDetail/内蒙古/呼伦贝尔牙克石.json)|
|[内蒙古_满洲里](./data/ChildDetail/内蒙古/满洲里.json)|
|[内蒙古_通辽](./data/ChildDetail/内蒙古/通辽.json)|
|[内蒙古_乌海](./data/ChildDetail/内蒙古/乌海.json)|
|[内蒙古_乌兰察布](./data/ChildDetail/内蒙古/乌兰察布.json)|
|[内蒙古_锡林郭勒](./data/ChildDetail/内蒙古/锡林郭勒.json)|
|[内蒙古_锡林郭勒盟](./data/ChildDetail/内蒙古/锡林郭勒盟.json)|
|[内蒙古_锡林郭勒盟二连浩特](./data/ChildDetail/内蒙古/锡林郭勒盟二连浩特.json)|
|[内蒙古_锡林郭勒盟锡林浩特](./data/ChildDetail/内蒙古/锡林郭勒盟锡林浩特.json)|
|[内蒙古_兴安盟](./data/ChildDetail/内蒙古/兴安盟.json)|
|[内蒙古_兴安盟乌兰浩特](./data/ChildDetail/内蒙古/兴安盟乌兰浩特.json)|
|[宁夏_待明确地区](./data/ChildDetail/宁夏/待明确地区.json)|
|[宁夏_固原](./data/ChildDetail/宁夏/固原.json)|
|[宁夏_宁东](./data/ChildDetail/宁夏/宁东.json)|
|[宁夏_宁东管委会](./data/ChildDetail/宁夏/宁东管委会.json)|
|[宁夏_石嘴山](./data/ChildDetail/宁夏/石嘴山.json)|
|[宁夏_吴忠](./data/ChildDetail/宁夏/吴忠.json)|
|[宁夏_银川](./data/ChildDetail/宁夏/银川.json)|
|[宁夏_中卫](./data/ChildDetail/宁夏/中卫.json)|
|[青海_北海](./data/ChildDetail/青海/北海.json)|
|[青海_待明确地区](./data/ChildDetail/青海/待明确地区.json)|
|[青海_海北](./data/ChildDetail/青海/海北.json)|
|[青海_西宁](./data/ChildDetail/青海/西宁.json)|
|[山东_滨州](./data/ChildDetail/山东/滨州.json)|
|[山东_待明确地区](./data/ChildDetail/山东/待明确地区.json)|
|[山东_德州](./data/ChildDetail/山东/德州.json)|
|[山东_菏泽](./data/ChildDetail/山东/菏泽.json)|
|[山东_济南](./data/ChildDetail/山东/济南.json)|
|[山东_济宁](./data/ChildDetail/山东/济宁.json)|
|[山东_聊城](./data/ChildDetail/山东/聊城.json)|
|[山东_临沂](./data/ChildDetail/山东/临沂.json)|
|[山东_青岛](./data/ChildDetail/山东/青岛.json)|
|[山东_任城监狱](./data/ChildDetail/山东/任城监狱.json)|
|[山东_日照](./data/ChildDetail/山东/日照.json)|
|[山东_泰安](./data/ChildDetail/山东/泰安.json)|
|[山东_威海](./data/ChildDetail/山东/威海.json)|
|[山东_潍坊](./data/ChildDetail/山东/潍坊.json)|
|[山东_烟台](./data/ChildDetail/山东/烟台.json)|
|[山东_枣庄](./data/ChildDetail/山东/枣庄.json)|
|[山东_淄博](./data/ChildDetail/山东/淄博.json)|
|[山西_大同](./data/ChildDetail/山西/大同.json)|
|[山西_晋城](./data/ChildDetail/山西/晋城.json)|
|[山西_晋中](./data/ChildDetail/山西/晋中.json)|
|[山西_临汾](./data/ChildDetail/山西/临汾.json)|
|[山西_吕梁](./data/ChildDetail/山西/吕梁.json)|
|[山西_朔州](./data/ChildDetail/山西/朔州.json)|
|[山西_太原](./data/ChildDetail/山西/太原.json)|
|[山西_忻州](./data/ChildDetail/山西/忻州.json)|
|[山西_阳泉](./data/ChildDetail/山西/阳泉.json)|
|[山西_运城](./data/ChildDetail/山西/运城.json)|
|[山西_长治](./data/ChildDetail/山西/长治.json)|
|[陕西_安康](./data/ChildDetail/陕西/安康.json)|
|[陕西_宝鸡](./data/ChildDetail/陕西/宝鸡.json)|
|[陕西_待明确地区](./data/ChildDetail/陕西/待明确地区.json)|
|[陕西_韩城](./data/ChildDetail/陕西/韩城.json)|
|[陕西_汉中](./data/ChildDetail/陕西/汉中.json)|
|[陕西_商洛](./data/ChildDetail/陕西/商洛.json)|
|[陕西_铜川](./data/ChildDetail/陕西/铜川.json)|
|[陕西_渭南](./data/ChildDetail/陕西/渭南.json)|
|[陕西_西安](./data/ChildDetail/陕西/西安.json)|
|[陕西_咸阳](./data/ChildDetail/陕西/咸阳.json)|
|[陕西_延安](./data/ChildDetail/陕西/延安.json)|
|[陕西_杨凌](./data/ChildDetail/陕西/杨凌.json)|
|[陕西_榆林](./data/ChildDetail/陕西/榆林.json)|
|[上海_宝山](./data/ChildDetail/上海/宝山.json)|
|[上海_崇明](./data/ChildDetail/上海/崇明.json)|
|[上海_待明确地区](./data/ChildDetail/上海/待明确地区.json)|
|[上海_奉贤](./data/ChildDetail/上海/奉贤.json)|
|[上海_虹口](./data/ChildDetail/上海/虹口.json)|
|[上海_黄浦](./data/ChildDetail/上海/黄浦.json)|
|[上海_嘉定](./data/ChildDetail/上海/嘉定.json)|
|[上海_金山](./data/ChildDetail/上海/金山.json)|
|[上海_静安](./data/ChildDetail/上海/静安.json)|
|[上海_闵行](./data/ChildDetail/上海/闵行.json)|
|[上海_浦东](./data/ChildDetail/上海/浦东.json)|
|[上海_普陀](./data/ChildDetail/上海/普陀.json)|
|[上海_青浦](./data/ChildDetail/上海/青浦.json)|
|[上海_松江](./data/ChildDetail/上海/松江.json)|
|[上海_外地来人员](./data/ChildDetail/上海/外地来人员.json)|
|[上海_徐汇](./data/ChildDetail/上海/徐汇.json)|
|[上海_杨浦](./data/ChildDetail/上海/杨浦.json)|
|[上海_长宁](./data/ChildDetail/上海/长宁.json)|
|[四川_阿坝](./data/ChildDetail/四川/阿坝.json)|
|[四川_巴中](./data/ChildDetail/四川/巴中.json)|
|[四川_成都](./data/ChildDetail/四川/成都.json)|
|[四川_达州](./data/ChildDetail/四川/达州.json)|
|[四川_待明确地区](./data/ChildDetail/四川/待明确地区.json)|
|[四川_德阳](./data/ChildDetail/四川/德阳.json)|
|[四川_甘孜](./data/ChildDetail/四川/甘孜.json)|
|[四川_广安](./data/ChildDetail/四川/广安.json)|
|[四川_广元](./data/ChildDetail/四川/广元.json)|
|[四川_乐山](./data/ChildDetail/四川/乐山.json)|
|[四川_凉山](./data/ChildDetail/四川/凉山.json)|
|[四川_泸州](./data/ChildDetail/四川/泸州.json)|
|[四川_眉山](./data/ChildDetail/四川/眉山.json)|
|[四川_绵阳](./data/ChildDetail/四川/绵阳.json)|
|[四川_南充](./data/ChildDetail/四川/南充.json)|
|[四川_内江](./data/ChildDetail/四川/内江.json)|
|[四川_攀枝花](./data/ChildDetail/四川/攀枝花.json)|
|[四川_遂宁](./data/ChildDetail/四川/遂宁.json)|
|[四川_雅安](./data/ChildDetail/四川/雅安.json)|
|[四川_宜宾](./data/ChildDetail/四川/宜宾.json)|
|[四川_资阳](./data/ChildDetail/四川/资阳.json)|
|[四川_自贡](./data/ChildDetail/四川/自贡.json)|
|[天津_宝坻](./data/ChildDetail/天津/宝坻.json)|
|[天津_北辰](./data/ChildDetail/天津/北辰.json)|
|[天津_滨海](./data/ChildDetail/天津/滨海.json)|
|[天津_待明确地区](./data/ChildDetail/天津/待明确地区.json)|
|[天津_东丽](./data/ChildDetail/天津/东丽.json)|
|[天津_和平](./data/ChildDetail/天津/和平.json)|
|[天津_河北](./data/ChildDetail/天津/河北.json)|
|[天津_河东](./data/ChildDetail/天津/河东.json)|
|[天津_河西](./data/ChildDetail/天津/河西.json)|
|[天津_红桥](./data/ChildDetail/天津/红桥.json)|
|[天津_津南](./data/ChildDetail/天津/津南.json)|
|[天津_南开](./data/ChildDetail/天津/南开.json)|
|[天津_宁河](./data/ChildDetail/天津/宁河.json)|
|[天津_外地来人员](./data/ChildDetail/天津/外地来人员.json)|
|[天津_武清](./data/ChildDetail/天津/武清.json)|
|[天津_西青](./data/ChildDetail/天津/西青.json)|
|[西藏_待明确地区](./data/ChildDetail/西藏/待明确地区.json)|
|[西藏_拉萨](./data/ChildDetail/西藏/拉萨.json)|
|[新疆_阿克苏](./data/ChildDetail/新疆/阿克苏.json)|
|[新疆_巴州](./data/ChildDetail/新疆/巴州.json)|
|[新疆_兵团第八师石河子](./data/ChildDetail/新疆/兵团第八师石河子.json)|
|[新疆_兵团第九师](./data/ChildDetail/新疆/兵团第九师.json)|
|[新疆_兵团第六师五家渠](./data/ChildDetail/新疆/兵团第六师五家渠.json)|
|[新疆_兵团第七师](./data/ChildDetail/新疆/兵团第七师.json)|
|[新疆_兵团第十二师](./data/ChildDetail/新疆/兵团第十二师.json)|
|[新疆_兵团第四师](./data/ChildDetail/新疆/兵团第四师.json)|
|[新疆_兵团第五师五家渠](./data/ChildDetail/新疆/兵团第五师五家渠.json)|
|[新疆_昌吉](./data/ChildDetail/新疆/昌吉.json)|
|[新疆_第八师](./data/ChildDetail/新疆/第八师.json)|
|[新疆_第八师石河子](./data/ChildDetail/新疆/第八师石河子.json)|
|[新疆_第九师](./data/ChildDetail/新疆/第九师.json)|
|[新疆_第六师](./data/ChildDetail/新疆/第六师.json)|
|[新疆_第七师](./data/ChildDetail/新疆/第七师.json)|
|[新疆_胡杨河](./data/ChildDetail/新疆/胡杨河.json)|
|[新疆_石河子](./data/ChildDetail/新疆/石河子.json)|
|[新疆_塔城](./data/ChildDetail/新疆/塔城.json)|
|[新疆_吐鲁番](./data/ChildDetail/新疆/吐鲁番.json)|
|[新疆_乌鲁木齐](./data/ChildDetail/新疆/乌鲁木齐.json)|
|[新疆_五家渠](./data/ChildDetail/新疆/五家渠.json)|
|[新疆_伊犁](./data/ChildDetail/新疆/伊犁.json)|
|[云南_保山](./data/ChildDetail/云南/保山.json)|
|[云南_楚雄](./data/ChildDetail/云南/楚雄.json)|
|[云南_大理](./data/ChildDetail/云南/大理.json)|
|[云南_待明确地区](./data/ChildDetail/云南/待明确地区.json)|
|[云南_德宏](./data/ChildDetail/云南/德宏.json)|
|[云南_红河](./data/ChildDetail/云南/红河.json)|
|[云南_昆明](./data/ChildDetail/云南/昆明.json)|
|[云南_丽江](./data/ChildDetail/云南/丽江.json)|
|[云南_临沧](./data/ChildDetail/云南/临沧.json)|
|[云南_普洱](./data/ChildDetail/云南/普洱.json)|
|[云南_曲靖](./data/ChildDetail/云南/曲靖.json)|
|[云南_文山](./data/ChildDetail/云南/文山.json)|
|[云南_西双版纳](./data/ChildDetail/云南/西双版纳.json)|
|[云南_玉溪](./data/ChildDetail/云南/玉溪.json)|
|[云南_昭通](./data/ChildDetail/云南/昭通.json)|
|[浙江_待明确地区](./data/ChildDetail/浙江/待明确地区.json)|
|[浙江_杭州](./data/ChildDetail/浙江/杭州.json)|
|[浙江_湖州](./data/ChildDetail/浙江/湖州.json)|
|[浙江_嘉兴](./data/ChildDetail/浙江/嘉兴.json)|
|[浙江_金华](./data/ChildDetail/浙江/金华.json)|
|[浙江_丽水](./data/ChildDetail/浙江/丽水.json)|
|[浙江_宁波](./data/ChildDetail/浙江/宁波.json)|
|[浙江_衢州](./data/ChildDetail/浙江/衢州.json)|
|[浙江_绍兴](./data/ChildDetail/浙江/绍兴.json)|
|[浙江_省十里丰监狱](./data/ChildDetail/浙江/省十里丰监狱.json)|
|[浙江_台州](./data/ChildDetail/浙江/台州.json)|
|[浙江_温州](./data/ChildDetail/浙江/温州.json)|
|[浙江_舟山](./data/ChildDetail/浙江/舟山.json)|
|[重庆_巴南](./data/ChildDetail/重庆/巴南.json)|
|[重庆_璧山](./data/ChildDetail/重庆/璧山.json)|
|[重庆_城口](./data/ChildDetail/重庆/城口.json)|
|[重庆_大渡口](./data/ChildDetail/重庆/大渡口.json)|
|[重庆_大足](./data/ChildDetail/重庆/大足.json)|
|[重庆_待明确地区](./data/ChildDetail/重庆/待明确地区.json)|
|[重庆_垫江](./data/ChildDetail/重庆/垫江.json)|
|[重庆_丰都](./data/ChildDetail/重庆/丰都.json)|
|[重庆_奉节](./data/ChildDetail/重庆/奉节.json)|
|[重庆_涪陵](./data/ChildDetail/重庆/涪陵.json)|
|[重庆_高新](./data/ChildDetail/重庆/高新.json)|
|[重庆_合川](./data/ChildDetail/重庆/合川.json)|
|[重庆_江北](./data/ChildDetail/重庆/江北.json)|
|[重庆_江津](./data/ChildDetail/重庆/江津.json)|
|[重庆_九龙坡区](./data/ChildDetail/重庆/九龙坡区.json)|
|[重庆_开州](./data/ChildDetail/重庆/开州.json)|
|[重庆_梁平](./data/ChildDetail/重庆/梁平.json)|
|[重庆_两江](./data/ChildDetail/重庆/两江.json)|
|[重庆_南岸](./data/ChildDetail/重庆/南岸.json)|
|[重庆_彭水](./data/ChildDetail/重庆/彭水.json)|
|[重庆_綦江](./data/ChildDetail/重庆/綦江.json)|
|[重庆_黔江](./data/ChildDetail/重庆/黔江.json)|
|[重庆_荣昌](./data/ChildDetail/重庆/荣昌.json)|
|[重庆_沙坪坝](./data/ChildDetail/重庆/沙坪坝.json)|
|[重庆_石柱](./data/ChildDetail/重庆/石柱.json)|
|[重庆_铜梁](./data/ChildDetail/重庆/铜梁.json)|
|[重庆_潼南](./data/ChildDetail/重庆/潼南.json)|
|[重庆_万盛经开区](./data/ChildDetail/重庆/万盛经开区.json)|
|[重庆_万州](./data/ChildDetail/重庆/万州.json)|
|[重庆_巫山](./data/ChildDetail/重庆/巫山.json)|
|[重庆_巫溪](./data/ChildDetail/重庆/巫溪.json)|
|[重庆_武隆](./data/ChildDetail/重庆/武隆.json)|
|[重庆_秀山](./data/ChildDetail/重庆/秀山.json)|
|[重庆_永川](./data/ChildDetail/重庆/永川.json)|
|[重庆_酉阳](./data/ChildDetail/重庆/酉阳.json)|
|[重庆_渝北](./data/ChildDetail/重庆/渝北.json)|
|[重庆_渝中](./data/ChildDetail/重庆/渝中.json)|
|[重庆_云阳](./data/ChildDetail/重庆/云阳.json)|
|[重庆_长寿](./data/ChildDetail/重庆/长寿.json)|
|[重庆_忠县](./data/ChildDetail/重庆/忠县.json)|

## 5.数据排序问题

中文有多音字的情况，比如重庆的“重”可能会按读音zhòng来进行排序，所以排序会有些问题。

## 6.一些个人的DXY-COVID-19数据分析心得

康复率，死亡率和政治治疗率需要合在一起考虑，若事件结束后最终康复率教高，早期阶段数据少会造成数据有很大波动，中间阶段死亡率会逐步上升，死亡率会缓慢上升，正在治疗率会逐步下降。以死亡率在中期阶段大数据情况下，这会使得较少数据“噪点”数据就出现较大数值变动成为历史，就会出现缓慢上升这个前提条件来看，整体而言，患者多的地区较容易出现高死亡率，北方比南方较容易出现较高死亡率，越冷就越如此，这和[最终统计的2003年北京的SARS的死亡率](https://zyq5945.github.io/zyq5945/blog_10.html)比广东的差是一致的。

瞎琢磨尝试用安徽省的康复数标准化数据进行Boltzmann数据拟合，还挺符合的。
