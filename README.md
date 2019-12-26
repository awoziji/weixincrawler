# scrapy-redis-weixincrawler
微信公众号爬虫(非搜狗接口)
利用微信读书入口爬取微信公众号文章

## 爬取原理
通过将微信公众号文章通过微信读书打开，可以获取到微信公众号下相关文章的链接，这样比通过搜狗接口能更快速的获取微信公众号最新的文章，也可以规避搜狗接口文章数的限制。
## 方法
> * 首先在手机上安装微信读书的app。
> * 通过charles或者Fiddle对手机的请求进行抓包，获取登录微信读书的相关参数。
> * 在手机上打开微信并打开需要抓取的公众号中的任意一篇文章，同时进行抓包，获取公众号文章抓取的URL。
> * 将相关参数添加到代码中进行爬取。

### 备注
> * 登录微信读书的相关参数抓包一次后可多次使用，但实际情况可能会出现过期或失效。
> * 此方法在9月2日测试依然可用。
