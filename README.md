# PHP-Waste-Sorting
PHP简单实现垃圾分类查询

前言

    自上海2019.7.1日起严格实施垃圾分类，萌发了很多垃圾分类查询应用，网上也没有找到API或开源代码所以准备自己简单实现下
请求示例

    http://localhost/index.php?kw=面

实现逻辑

    主要逻辑是读取文本内容并打上ID标签，并通过GET提交过来的KW参数进行正则2次匹配
    

优化方案

    方案1，通过用户前端提交分类，后台工作人员进行审核词库。效率较低，准确度低
    方案2，通过工作人员手动更新分类词库。效率一般，需要大量人力
    方案3，通过机器学习，定义多个指标如物品的类型，可食用性，湿度，外形来判断是属于哪一类垃圾。效率高，需要研发成本
