# code_space_spider_demo
爬虫核心三个模块：URL管理器，网页下载器，网页解析器。三者形成一个循环，只要有URL可下载，就一直运行下去，直到爬遍整个待爬网站。

- URL管理器：对将要爬取的URL和已经爬取的URL进行管理。
- 网页下载器：接受URL管理器发送过来的待爬取的URL，然后把该URL对应的网页下载并存储下来。
- 网页解析器：网页下载器下载下来的网页交给网页解析器进行解析，一方面解析出有价值的数据，另一方面解析出网页上所有的URL，补充进URL管理器。

### 项目结构
```python
code_space_spider_demo
   ├─html_downloader.py		网页下载器
   ├─html_outputer.py		数据处理器
   ├─html_parser.py		网页解析器
   ├─output.html		数据展示html
   ├─spider_main.py		爬虫启动器
   ├─urls_manager.py		URL管理器
```
爬虫调度端：启动，停止爬虫，监视爬虫的运行情况。
