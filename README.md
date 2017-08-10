# loading demo

### demo1 使用定时器实现loading动画
**优点：** 简单粗暴，一个gif搞定

**缺点：** 假的进度条，没有真实反映进度。特别是有缓存的时候，每次刷新还是会停留同样的时间。

**效果：**
![](https://ws1.sinaimg.cn/large/006tNc79gy1fies7ynm0ng30ao05twuk.gif)



### demo2 根据加载状态判断进度，实现loading动画
**优点：** loading动画的消失时间比较准确。

**缺点：** 不能实时反映加载进度

**效果：**
![](https://ws4.sinaimg.cn/large/006tNc79gy1fies84hh9ag30a604rtb5.gif)


### demo3 与demo2一致，不过动画是使用CSS3写的
**优点：** 不用gif图片，更加轻巧

**缺点：** 不能实时反映加载进度

**效果：**
![](https://ws1.sinaimg.cn/large/006tNc79gy1fies8dzugeg308c04n75o.gif)


### demo4 定位在头部的loading动画
将script插入到html文档的不同位置，并设置进度条的进度即可。基本原理：浏览器执行代码是从上到下运行的。

**优点：** 高大上的感觉，现在很多网站都用这种，比较实时反映加载的进度

**缺点：** 在html中插入多处脚本，容易导致html文档的紊乱，结构不清晰。

**效果：** 
![](https://ws3.sinaimg.cn/large/006tNc79gy1fies8mcgx3g30av061q8i.gif)

### demo5 据图像的加载进度，实时获取加载数据的进度条。
**优点：** 比较准确反映了加载的进度，还可实时看到加载的百分比。对DOM结构也没有构成破坏。

**缺点：** 进度是根据图片的加载进度来反映的，如果网站中不是图片占主导，就不是很准确。但已经是比较好的方法 了，进度条嘛，给大家打发时间的~~

**效果：** 
![](https://ws1.sinaimg.cn/large/006tNc79gy1fies8ywl32g307x048k14.gif)


