# 微博收藏夹图片爬虫

## How to run

#### 0. Clone the project

#### 1. 新建images图片文件夹, under the root folder

#### 2. 新建config文件夹

#### 3. 在config文件夹下新建index.js文件
内容如下:
```javascript
exports.cookies = '' // https://m.weibo.cn 登录后的cookies
exports.containerid = '' // https://m.weibo.cn/ => 我 => 我的收藏 => 地址栏上的containerid
```
注意使用微博移动网页版的接口，目前版本containerid并不在地址栏上显示，它和Cookie都需要打开开发者视图，注意https://m.weibo.cn/api/container/getIndex这个请求，Cookie可以通过导出curl看到。

#### 4. Run

```bash
$yarn
#or
$npm install
$npm run dev
```
