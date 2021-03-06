
## 土豆搜索引擎<br>
<a href="https://search.littlepotato.life/">https://search.littlepotato.life/</a><br>

#### 使用谷歌自定义搜索，返回搜索结果。<br>
使用了 Django 框架，<b>表单</b>获取用户输入，<b>视图</b>将用户输入的内容构造成<b>请求URL</b>，向<b>谷歌API</b>进行请求，拿到结果后进行提取，再把提取后的内容交由<b>视图</b>处理后写入<b>模板</b>并返回前端页面。<br>

### 特色功能
<b>搜索</b>：搜索结果与谷歌相同，在中国大陆地区可用，不会搜集用户信息。<br>
<b>搜书</b>：去特定的电子书下载网站搜索你要的书籍，帮你找到想要的电子书。<br>
<b>匿名访问</b>：通过 Web 代理打开目标网页，能在不使用任何软件的情况下访问中国大陆地区无法访问的网站（使用 <a href="https://github.com/EtherDream/jsproxy">jsproxy</a> 部署在 Cloudflare Workers）。<br>
<b>语言选择</b>：能在“搜索结果”页面方便的切换语言，使搜索结果更趋向于你所选择的语言（目前支持 英文、简体中文、 繁体中文）。<br>
<b>APPS</b>：提供多种便捷的网页版工具，节省您的时间（还在逐步开发中）。<br>

![搜索引擎](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/index.png)
<hr>

![搜索结果1](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/detail1.png)
<hr>

![搜索结果2](https://raw.githubusercontent.com/justsweetpotato/markdown-img-store/master/search/detail2.png)

### 版本更新
<b>v1.0.0</b> (03/26/2020)<br>
修改了结果展示的逻辑，现在默认以原始权重排列结果，不在强制以语言排列结果。<br>
修复了一些问题。<br>

<b>v0.3.4</b> (11/16/2019)<br>
分页功能完善，API 功能完善，修复多处手机端页面排版问题。<br>

<details>
  <summary>显示更多</summary>
<b>v0.3.3</b> (9/23/2019)<br>
新增繁体中文界面，优化了切换语言的逻辑，多语言界面的切换将更顺畅。<br>
主页左上角新增 APPS 功能，集成多种便捷网页版工具。<br>
<br>
  
<b>v0.3.2</b> (8/23/2019)<br>
性能优化，使用多线程完成请求，减少页面等待时间。<br>
页面优化，分离电脑端与手机端页面，提升用户体验度。<br>
新增英语界面，搜索结果无缝切换。<br>
其他多项优化。<br>

<b>v0.3.1</b> (8/1/2019)<br>
除“搜书”功能外增加“搜索”功能，搜索结果与谷歌相同。<br>
增加“词条简介”，搜索结果会出现来自维基百科的简介（如果有的话）。<br>
增加以“沙盒模式”打开网页，通过内置的“网页代理”访问网站，能直接访问中国大陆无法访问的网站。<br>
在页面底部增加“定位”开关，默认关闭状态（开启会略微增加网页响应时间）。<br>

<b>v0.3.0 正式版</b> (7/24/2019)<br>
完成分页功能。<br>
大幅度优化界面显示。<br>

<b>v0.2.4</b> (7/23/2019)<br>
搜索详情界面优化，现在可以在详情页面进行搜索。<br>
搜索结果增加了详细说明。<br>
优化了代码逻辑，更加简洁美观。<br>

<b>v0.2.3</b> (4/2/2019)<br>
修复了界面文本的一些错误，对用户使用更加友好。<br> 
优化了向 API 发送请求的逻辑，现在会自动关闭连接。<br>

<b>v0.2.2</b> (3/31/2019)<br>
在谷歌 CSE 平台更新了书籍搜索源（旧搜索源有些已经无法访问，已删除无法访问的源并新增源）。<br>

<b>v0.2.1</b> <br>
新增了一个 APIKEY 配额用尽时的提示。<br> 
新增了 404 页面与 500 页面。<br>
解决了搜索一串乱码时，服务器返回 403 的错误（现在会显示未搜索到内容）。<br>
已知问题：分页功能未完成，目前只显示 1 页 10 条结果。<br>

<b>v0.2.0 正式版</b> <br>
在 青空锁云 的帮助下完成了数据提取部分，调用谷歌 API 返回数据提取后填充到网页中，解决了中国大陆无法访问的问题！<br>

<b>v0.1.1</b> <br>
增加了随机显示名人名言，优化了页面排版。<br>
已知问题：中国大陆无法使用。<br>

<b>v0.1.0</b> <br>
基础引擎框架。<br>
已知问题：中国大陆无法使用（谷歌提供的 JavaScript 代码无法正常加载，并且反向代理无法解决这个问题）。<br>
</details>
