# csdn
## 项目整体使用的渲染技术是vue。简单的实现了查看文章详情；关注博主（取消关注博主）；收藏文章（取消收藏文章）；发布文章；编辑修改发布的文章；删除发布的文章等功能。
>1查看文章详情：<br>
需要从首页传一个文章的id号，然后根据文章id号取到文章内容。
文章的id号用是地址栏传参的方式从首页传过来的，在详情页对地址栏进行解析得到id号（解析方式是用split进行解析，window.location.search.split("=")[1]，用split将地址栏参数用“=”号分隔开，然后取数组里的第一位[数组默认从第0位开始]，即为所要的id号）。然后用ajax的方法取到数据
