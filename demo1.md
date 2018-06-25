H1
====
H2
----

#### H4
##### H5

>引用内容

>如果仅在第一行使用`>`,
后面相邻的行即使省略`>`, 也会变成引用内容。

>如果引用内容需要换行，  
>可以在行尾添加两个空格
>
>或者在引用内容中加一个空行

>也可以在引用中
>>使用嵌套的引用

>在引用中可以使用其他任何*Markdown*语法

* 可以使用`*`作为标记
+ 也可以使用`+`
- 或者`-`

1. 有序列表以数字和`.`开始；
3. 数字的序列并不会影响生成的列表序列；
4. 但仍然推荐按照自然顺序(1.2.3...)编写。

### 嵌套的列表
1. 第一层
    + 1-1
    + 1-2
2. 无序列表和有序列表可以随意相互嵌套
    1. 2-1
    2. 2-2

05\. 可以使用: 数字\\.来取消显示为列表

	<html>  // Tab开头
        <title>Markdown</title>
    </html> // 四个空格开头

行内代码，例如`<title>Markdown</title>`

***
------
___

* * *
- - -

# 超链接
## 行内式
格式为\[link text\](url 'title text')。

①普通链接：
[Google](http://www.google.com/)

②指向本地文件的链接：
[icon.png](./images/icon.png)

③包含'title'的链接
[Google](http://www.google.com/ "Google")
>title使用'或"都是可以的。

## 参考式
①首先，定义链接：

[Google][link]

②然后定义链接内容：

[link]: http://www.google.com/ 'Google'

③也可以省略 识别符，使用链接文本作为 识别符：

[Google][]

[Google]: http://www.google.com/ 'Google'

## 自动链接
使用 <> 包括的 URL 或邮箱地址会被自动转换为超链接：  
<http://www.google.com/>  
<123@email.com>

# 图像
插入图片的语法和插入超链接的语法基本一致，只是在最前面多一个 !。也分为行内式和参考式两种。
## 行内式
![GitHub](https://avatars2.githubusercontent.com/u/3265208?v=3&s=100 "GitHub,Social Coding")
<!-- ![GitHub](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1529844184431&di=4dd5bf8b9a926fc61a3848345963af6e&imgtype=0&src=http%3A%2F%2Fimgsrc.baidu.com%2Fforum%2Fw%3D580%2Fsign%3D9715010d942f07085f052a08d925b865%2Fbbb44faccbef76095bf58add24dda3cc7dd99eb3.jpg "樱空桃") -->

## 参考式
![GitHub][github]

[github]: https://avatars2.githubusercontent.com/u/3265208?v=3&s=100 "GitHub,Social Coding"

## 指定图片的显示大小
<img src="https://avatars2.githubusercontent.com/u/3265208?v=3&s=100" alt="GitHub" title="GitHub,Social Coding" width="50" height="50" />

# 强调
1. 使用 * * 或 _ _ 包括的文本会被转换为 `<em></em>` ，通常表现为斜体：  
这是用来 *演示* 的 _文本_
2. 使用 ** ** 或 __ __ 包括的文本会被转换为 `<strong></strong>`，通常表现为加粗：  
这是用来 **演示** 的 __文本__
3. 用来包括文本的 * 或 _ 内侧不能有空白，否则 * 和 _ 将不会被转换（不同的实现会有不同的表现）：  
这是用来 * 演示* 的 _文本 _
4. 如果需要在文本中显示成对的 * 或 _，可以在符号前加入 \ 即可：  
这是用来 \*演示\* 的 \_文本\_
5. *、**、_ 和 __ 都必须 成对使用。

# 删除线
这就是 ~~删除线~~

# 代码块和语法高亮
## 代码块
```
<p>code here</p>
```

## 语法高亮
```js
window.addEventListener('load', function() {
    console.log('window loaded');
});
```

# 表格
## 单元格和表头
| name       | age |
| ---------- | --- |
| LearnShare | 12  |
| Mike       | 32  |

| name       | age |
| ---------- | --- |
| LearnShare | 12  |
| Mike       | 32  |

## 对齐
| left | center | right |
| :--- | :----: | ----: |
| aaaa | bbbbbb | ccccc |
| a    | b      | c     |

## 插入其他内容
| name         | age   | blog                            |
| ------------ | :---: | ------------------------------: |
| _LearnShare_ | 12    | [LearnShare](http://xianbai.me) |
| __Mike__     | 32    | [Mike](http://mike.me)          |

# Task List
- [ ] Eat
- [x] Code
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] Sleep

$$ \frac{d}{dx}e^{ax}=ae^{ax}\quad \sum_{i=1}^{n}{(X_i - \overline{X})^2} $$