# advanced-php-crawler
## 新浪博客全能爬虫
这套PHP编写的小程序可以帮助喜欢在电子书阅读器上看新浪博客上文章的你，它可以根据已知的文章列表来爬行，亦可以根据已知的文章目录来爬行，还可以与Calibre等工具配合生成带目录的电子书。文章细节均已自动优化，且使用MarkDown格式，只为带给你完美的阅读体验！
## 文件功能详解：
### sina-list.php
它用于爬行像这样子的博客文章目录：
![][image-1]

>  新浪博客爬虫-列表爬虫`<br/>`
> -可以集合已知文章目录（/s/articlelist*）里面的文章列表`<br/>`
> 使用方法：`<br/>`
> php sina-list.php \<网址文件\> `<br/>`
> 参数解释：`<br/>`
> \<网址文件\>：一行一个网址，请使用电脑版访问后复制`<br/>`
> 命令示例：`<br/>`
> php sina-list.php urls.txt `<br/>`
> 网址文件示例：`<br/>`
> http://blog.sina.com.cn/s/articlelist_123456wsla.html `<br/>`
> http://blog.sina.com.cn/s/articlelist_789456wsex.html `<br/>`

### sina-article.php
它用于爬行像这样子的具体文章：
![][image-2]

> 新浪博客爬虫-文章爬虫`<br/>`
> -可以提取已知文章页面（/s/blog*）里面的文章`<br/>`
> 使用方法：`<br/>`
> php sina-article.php \<网址文件\> `<br/>`
> 参数解释：`<br/>`
> \<网址文件\>：一行一个网址，请使用电脑版访问后复制`<br/>`
> 命令示例：`<br/>`
> php sina-article.php urls.txt `<br/>`
> 网址文件示例：`<br/>`
> http://blog.sina.com.cn/s/blog_123456wsla.html `<br/>`
> http://blog.sina.com.cn/s/blog_789456wsex.html `<br/>`

### tool-rev.php
它用于把上面说的网址文件前前后后颠倒过来
> 新浪博客爬虫-网址文件反转工具`<br/>`
> -将某个网址文件里面的url全部反转过来，可用于处理新旧文章顺序等`<br/>`
> 使用方法：`<br/>`
> php tool-rev.php \<网址文件\> `<br/>`
> 参数解释：`<br/>`
> \<网址文件\>：一行一个网址，请使用电脑版访问后复制`<br/>`
> 命令示例：`<br/>`
> php tool-rev.php urls.txt `<br/>`
> 网址文件示例：`<br/>`
> http://blog.sina.com.cn/s/xxx_123456wsla.html `<br/>`
> http://blog.sina.com.cn/s/xxx_789456wsex.html `<br/>`

## 附录
[Calibre：kindle后续成书步骤][1]

[1]:	https://kindlefere.com/post/82.html

[image-1]:	https://ww2.sinaimg.cn/large/006tNbRwgy1fdizlqnd8qj30s40i30wu.jpg
[image-2]:	https://ww1.sinaimg.cn/large/006tNbRwgy1fdizoxf1ivj30i40m7tgl.jpg