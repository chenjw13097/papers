# Word文档转Markdown文档的过程

首先，使用在线转换器[http://word-to-markdown.herokuapp.com/](http://word-to-markdown.herokuapp.com/)，将Word文档转换为Markdown文档。

此Markdown文档有些语法是GitHub不支持的（笔者暂未找到GitHub提供的转换器），需要作如下转换：
```
1）~是删除线的语法，需要转义（正则表达式）
~
\~
```

补充GitHub上Markdown的语法：
[https://guides.github.com/features/mastering-markdown/](https://guides.github.com/features/mastering-markdown/)
```
1）字体加粗
**bold**
2）斜体字
*italic*
3）网页链接
[link to Google!](http://google.com)
4）要点
* Start a line with a star
- Dashes work just as well
5)子要点
  - Like this
6）引用
> Coffee. The finest organic suspension ever devised... I beat the Borg with it.
> - Captain Janeway
7）带分割线的1号标题
# Structured documents
8）不带分割线的3号标题
### Structured documents
9）4个空格前导为缩进格式
    if (isAwesome){
      return true
    }
10）代码引用
```
或
```javascript
```