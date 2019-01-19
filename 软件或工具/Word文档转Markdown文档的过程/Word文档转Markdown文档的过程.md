# Word文档转Markdown文档的过程

**欢迎转载，但须指明出处：**[https://github.com/chenjw13097/papers](https://github.com/chenjw13097/papers/blob/master/%E8%BD%AF%E4%BB%B6%E6%88%96%E5%B7%A5%E5%85%B7/Word%E6%96%87%E6%A1%A3%E8%BD%ACMarkdown%E6%96%87%E6%A1%A3%E7%9A%84%E8%BF%87%E7%A8%8B/Word%E6%96%87%E6%A1%A3%E8%BD%ACMarkdown%E6%96%87%E6%A1%A3%E7%9A%84%E8%BF%87%E7%A8%8B.md)  

首先，使用在线转换器[http://word-to-markdown.herokuapp.com/](http://word-to-markdown.herokuapp.com/)，将Word文档转换为Markdown文档。  

此Markdown文档有些语法是GitHub不支持的（笔者暂未找到GitHub提供的转换器），需要作如下转换：  
```
1）~是删除线的语法，需要转义（Notepad++，正则表达式）
~
\~
```

补充GitHub上Markdown的语法：  
[https://guides.github.com/features/mastering-markdown/](https://guides.github.com/features/mastering-markdown/)  
[https://github.com/waylau/github-help/blob/master/GitHub%20Flavored%20Markdown.md](https://github.com/waylau/github-help/blob/master/GitHub%20Flavored%20Markdown.md)  
```
1）字体加粗
**bold**
2）斜体字
*italic*
3）链接
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
\```
或
\```javascript
11)转义Markdown特殊字符，如~
\\~
```