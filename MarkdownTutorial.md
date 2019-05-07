__页面内容__

* [1 文本](#1)
	* [1.1 标题](#11)
	* [1.2 加强和强调](#12)
	* [1.3 列表](#13)
		* [1.3.1 无序](#131)
		* [1.3.2 有序](#132)
	* [1.4 块引用](#14)
	* [1.5 链接](#15)
	* [1.6 内置代码](#16)
* [2 代码](#2)
* [3 图片](#3)
* [4 任务列表](#4)
* [5 表格](#5)
* [6 SHA引用](#6-sha)
* [7 Issue引用](#7-issue)
* [8 其他](#8)
    * [8.1 分割线](#81)
    * [8.2 提到用户名](#82)
    * [8.3 Emoji](#83-emoji)


# <div style="width: 100%; border-bottom: 1px solid;">1 文本</div>

使用Markdown用来**加粗**或*加斜体*文本是非常方便的，也可以加上
> 引文效果

或是加上放置列表

* 项目1
* 项目2

也可以连接到外部链接[Github](www.github.com)

## <div style="width: 100%; border-bottom: 1px dashed;">1.1 标题</div>

__效果__

># 一号标题
>## 二号标题
>###### 六号标题

__用法__

```
  # 一号标题
  ## 二号标题
  ###### 六号标题
```

## <div style="width: 100%; border-bottom: 1px dashed;">1.2 加强和强调</div>

__效果__

>*这是斜体效果*<br/>
>**这是加粗效果**<br/>
>__这是*混合*使用效果__<br/>
>_这是**混合**使用效果_<br/>
>~~这是删除线~~

__用法__

```
  *这是斜体效果*
  _这是斜体效果_

  **这是加粗效果**
  __这是加粗效果__

  __这是*混合*使用效果__
  **这是*混合*使用效果**   // 可以同时使用*和**，不能同时使用_和__

  _这是**混合**使用效果_<br/>

  ~~这是删除线~~
  <del>这是删除线</del>

```

## <div style="width: 100%; border-bottom: 1px dashed;">1.3 列表</div>
### <div style="width: 100%; border-bottom: 1px dotted;">1.3.1 无序</div>

__效果__

>* 项目1
>* 项目2
>		* 项目2.1
>		* 项目2.2

__使用__
```
  * 项目1
  * 项目2
  	* 项目2.1 // TAB键缩进
  	* 项目2.2

  或是
  - 项目1
  - 项目2
  	- 项目2.1
  	- 项目2.2
```

### <div style="width: 100%; border-bottom: 1px dotted;">1.3.2 有序</div>

__效果__

>1. 项目1
>1. 项目2
>		1. 项目2.1
>		1. 项目2.2


__使用__

```
  1. 项目1
  1. 项目2
  		1. 项目2.1 // 可以使用任意数字标示，使用TAB键缩进
  		1. 项目2.2
```

## <div style="width: 100%; border-bottom: 1px dashed;">1.4 块引用</div>

__效果__

> 块引用效果
>> 嵌套引用

__使用__

```
  > 块引用效果
  >> 嵌套引用
```

## <div style="width: 100%; border-bottom: 1px dashed;">1.5 链接</div>

__效果__

>http://github.com - automatic!<br/>
>[GitHub](http://github.com)

__使用__

```
  http://github.com - automatic!
  [GitHub](http://github.com)
```

## <div style="width: 100%; border-bottom: 1px dashed;">1.6 内置代码</div>

__效果__

> 可以使用内置代码元素`<span>`

__使用__

```
  可以使用内置代码元素`<span>`
```



# <div style="width: 100%; border-bottom: 1px solid;">2 代码</div>

__效果__

```
public void sayHello() {
	System.out.println("helloword")
}
```

```java
public void sayHello() {
	System.out.println("helloword")
}
```

__使用__

```
    // 使用四个空格缩进
        public void sayHello() {
	        System.out.println("helloword")
        }

    // 或是使用代码栅栏
	```
	public void sayHello() {
		System.out.println("helloword")
	}
	```

    // 如果需要语法高亮需要加上相应的语言标识
	```java
	public void sayHello() {
		System.out.println("helloword")
	}
	```

```


# <div style="width: 100%; border-bottom: 1px solid;">3 图片</div>

__效果__

![Image Of Cat](./images/cat1.jpg)

__用法__

```
	![Image Of Cat](./images/cat1.jpg)
```


# <div style="width: 100%; border-bottom: 1px solid;">4 任务列表</div>

__效果__

- [x] 支持@mention, #ref, [links](), **formatting**, <del>tag</del>
- [x] 要求列表语法
- [x] 这是完成的任务
- [ ] 这是未完成的任务

__使用__

```
	- [x] 支持@mention, #ref, [links](), **formatting**, <del>tag</del>
	- [x] 要求列表语法
	- [x] 这是完成的任务
	- [ ] 这是未完成的任务
```


# <div style="width: 100%; border-bottom: 1px solid;">5 表格</div>

__效果__

  第一个表格头 | 第二个表格头
  ---------- | ----------
  第一个单元格 | 第二个单元格
  第三个单元格 | 第四个单元格


__使用__

```
  // 第一行需要使用破折号- 列之间间隔使用分割线|

  第一个表格头 | 第二个表格头
  ---------- | ----------
  第一个单元格 | 第二个单元格
  第三个单元格 | 第四个单元格
```

# <div style="width: 100%; border-bottom: 1px solid;">6  SHA引用</div>

__效果__

mikepenz/MaterialDrawer@f4fb31635767edead0a01cee7b7588942b89d8d9

__使用__

```
  // Github 内部引用commit SHA-1
  f4fb31635767edead0a01cee7b7588942b89d8d9
  mikepenz@f4fb31635767edead0a01cee7b7588942b89d8d9

  // 可以在Github 之外引用commit SHA-1
  mikepenz/MaterialDrawer@f4fb31635767edead0a01cee7b7588942b89d8d9
```

# <div style="width: 100%; border-bottom: 1px solid;">7 Issue引用</div>

__效果__

mikepenz/MaterialDrawer#2446

__使用__

```
  // Github 内部引用issue
  #2446
  mikepenz#2446

  // Github 外部引用issue
  mikepenz/MaterialDrawer#2446
```

# <div style="width: 100%; border-bottom: 1px solid;">8 其他</div>
## <div style="width: 100%; border-bottom: 1px dashed;">8.1 分割线</div>

__效果__

*** 

__使用__

```
  ***
  或
  ---
  或
  ___
```

## <div style="width: 100%; border-bottom: 1px dashed;">8.2 提到用户名</div>

__效果__

@Username

__使用__

```
  @Username 提及某个用户名或是团队
```

## <div style="width: 100%; border-bottom: 1px dashed;">8.3 Emoji</div>

参看[Emoji](Emoji.md)
