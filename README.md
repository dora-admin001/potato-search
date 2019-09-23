
## 土豆搜索引擎<br>
<a href="https://search.littlepotato.life/">https://search.littlepotato.life/</a><br>

#### 使用谷歌自定义搜索, 返回搜索结果. <br>
使用了 Django 框架, <b>表单</b>获取用户输入, <b>视图</b>将用户输入的内容构造成<b>请求URL</b>, 向<b>谷歌API</b>进行请求, 拿到结果后进行提取, 再把提取后的内容交由<b>视图</b>处理后写入<b>模板</b>并返回前端页面. <br>

![搜索引擎](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/index.png)
<hr>

![搜索结果1](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/detail1.png)
<hr>

![搜索结果2](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/detail2.png)

### 版本更新
v3.2 (8/23/2019)<br>
性能优化, 使用多线程完成请求, 减少页面等待时间.<br>
页面优化, 分离电脑端与手机端页面, 提升用户体验度.<br>
中英双语界面, 搜索结果无缝切换.<br>
其他多项优化.<br>

v3.1 (8/1/2019)<br>
除"搜书功能"外增加"搜索功能", 搜索结果与谷歌相同.<br>
增加"词条简介"功能, 搜索结果会出现来自维基百科的简介(如果有的话).<br>
增加以"沙盒模式"打开网页, 通过内置的"网页代理"用户的真实 IP 将对目标网站隐藏.<br>
在页面底部增加"定位"开关, 默认关闭状态(开启会略微增加网页响应速度).

v3.0 正式版(7/24/2019)<br>
完成分页功能.<br>
大幅度优化界面显示.

v2.4 (7/23/2019)<br>
搜索详情界面优化, 现在可以在详情页面进行搜索.<br>
搜索结果增加了详细说明.<br>
优化了代码逻辑, 更加简洁美观.<br>

v2.3 (4/2/2019)<br>
修复了界面文本的一些错误, 对用户使用更加友好.<br> 
优化了向 API 发送请求的逻辑, 现在会自动关闭连接.

v2.2 (3/31/2019)<br>
在谷歌 CSE 平台更新了搜索源(旧搜索源有些已经无法访问, 已删除无法访问的源并新增源).

v2.1<br>
新增了一个 APIKEY 配额用尽时的提示.<br> 
新增了 404 页面与 500 页面.<br>
解决了搜索一串乱码时, 服务器返回 403 的错误(现在会显示未搜索到内容).<br>
已知问题: 分页功能未完成, 目前只显示 1 页 10 条结果.

v2.0 正式版<br>
在 青空锁云 的帮助下完成了数据提取部分, 调用谷歌 api 返回数据提取后填充到网页中, 解决了中国大陆无法访问的问题!

v1.1<br>
增加了随机显示名人名言 优化了页面排版.<br>
已知问题: 中国大陆无法使用.

v1.0<br>
基础引擎框架.<br>
已知问题: 中国大陆无法使用(谷歌 javascript 生成的界面在中国大陆无法加载, 并且反向代理无法解决这个问题).<br>
