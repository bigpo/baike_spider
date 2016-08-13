# 慕课网开发轻量级爬虫的代码

主要修改两处：
+ 模块spider_main 中异常处理部分：`except Exception as f:   print 'crew failed: ', f` 这样可以更容易定位错误。
+ 模块html_outputer 中，在`fout.('<html>')` 下面一行添加 `fout.write("<head><meta http-equiv='content-type' content='text/html;charset=utf-8'></head>")` 这个是解决中文乱码问题。
