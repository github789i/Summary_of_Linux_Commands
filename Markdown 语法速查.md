# Markdown 语法速查 

# 

>  25/12/7

## 1. 标题（Heading）

使用 `#`，后面要加 **空格**。

```markdown
# 一级标题
## 二级标题
### 三级标题
```

------

##  2. 换行（Line Break）

方式 1（推荐）：
 行末添加 **两个空格** + 回车

方式 2：

```markdown
<br>
```

------

##  3. 粗体（Bold）

```markdown
**word**
```

------

##  4. 斜体（Italic）

```markdown
*word*
```

------

##  5. 引用（Blockquote）

```markdown
> 引用
>> 嵌套引用
```

------

##  6. 有序列表（Ordered List）

数字 + 英文句点：

```markdown
1. item
2. item
```

------

##  7. 无序列表（Unordered List）

以下符号都可以使用：

```markdown
- item
* item
+ item
```

------

##  8. 行内代码（Inline Code）

反引号：

```markdown
`code`
```

多行代码（代码块）：

<pre> ```python print("Hello") ``` </pre> 

------

##  9. 分隔线（Horizontal Rule）

三个或以上的 `*` / `-` / `_`
 **前后都要有空行**

```markdown
---
***
___
```

------

##  10. 链接（Links）

普通链接：

```markdown
[name](link)
```

带 title（鼠标悬停提示）：

```markdown
[name](link "title")
```

自动链接：

```markdown
<https://example.com>
```

------

##  11. 图片（Images）

基本写法：

```markdown
![name](link "title")
```

点击图片跳转链接：

```markdown
[![name](image_link "title")](target_link)
```

------

##  12. 转义字符（Escape）

使用反斜杠 `\` 转义 Markdown 语法符号：

```markdown
\*word\*
```

------

##  13. 表格（Tables）

Markdown 原生表格格式较繁琐，通常使用在线工具生成：

```markdown
| Name | Age |
|------|-----|
| Tom  | 18  |
| Ann  | 20  |
```

常用生成网站：

- tablesgenerator.com
- online-markdown-editor