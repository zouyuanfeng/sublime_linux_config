### sublime text 3 linux 环境的配置
#### [中文的支持](http://jingyan.baidu.com/article/f3ad7d0ff8731609c3345b3b.html)
复制so库到安装目录下
```
$sudo mv libsublime-imfix.so /opt/sublime_text/
```
修改subl脚本，在/usr/bin/subl中
```
#!/bin/sh
LD_PRELOAD=/opt/sublime_text/libsublime-imfix.so exec /opt/sublime_text/sublime_text "$@"
```

#### [Markdown Preview 插件](http://jingyan.baidu.com/article/f006222838bac2fbd2f0c87d.html?st=2&net_type=&bd_page_type=1&os=0&rst=&word=feifeidown)
自定义快捷键
直接在浏览器中预览效果的话，可以自定义快捷键：点击 Preferences --> 选择 Key Bindings User，输入：
{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} },
保存后，直接输入快捷键：Alt + M 就可以直接在浏览器中预览生成的HTML文件了。

#### JsFormat
快捷键：ctrl+alt+f

