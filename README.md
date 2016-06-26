guoru restful-web-api

基于Node.js Express文件的增删改查REST API
请完成实现下列需求的一个简单的web-api

简单介绍
使用Node.js Express框架开发的对于文件的增删改查的REST API，通过Postman模拟客户对信息的增删改查以及返回所需要的数据和状态码
默认监听8010端口 部署前请使用 npm install 安装所需的依赖包！

用户相关

1. 获取所有数据信息
完整路径： http://localhsot:8010/products
支持方法： get
返回格式为JSON, 形式如下:
{
"id": 13,
"barcode": "ITEM000005",
"name": "qqq",
"unit": "袋",
"price": 4
}

2： 获取所有数据信息
完整路径： http://localhsot:8010/products/：id
支持方法： get
返回格式为JSON, 形式如下:
{
"id": 13,
"barcode": "ITEM000005",
"name": "qqq",
"unit": "袋",
"price": 4
}

3:插入数据
完整路径： http://localhsot:8010/products 
支持方法： post
返回格式为JSON, 形式如下:

{
  "barcode": "ITEM000005",
  "name": "qqq",
  "unit": "袋",
  "price": 4
}

4. 更新一条数据
完整路径：  http://localhsot:8010/products/:id
支持方法： put
在body里面输入要更新的JSON信息，比如:

{
  "barcode": "ITEM000005",
  "name": "qqq",
  "unit": "袋",
  "price": 4
}

5. 删除一条数据

完整路径： http://localhsot:8010/products/:id
支持方法： delete

*************
所有操作结果的都需返回状态玛。