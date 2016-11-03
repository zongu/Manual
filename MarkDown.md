# Markdown語法簡介
## 標題

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
## 換行與段落
* 一個換行字元會轉成換行`<br />`
* 兩個換行字元會轉成段落`<p></p>`

```markdown
第一段
第一行
第二行

第二段
第一行
第二行
```

## 字體
```markdown
*斜體*
**粗體**
***粗斜體***
~~刪除線~~
```

## 引言
```markdown
> 用>和一個空白表示
>> 多個>表示嵌套
```

## 水平分隔線
```markdown
三個以上的星號、連字號、底線表示
不能有空白或其他的文字
***
---
___
```

## 無序清單
```markdown
* 星號加空白
    * 加Tab可嵌套清單
+ 加號也可以
- 減號也可以
```

## 有序清單
```markdown
1. 格式為一個數字加小數點加空白
2. 數字本身順序不重要會自動遞增
    1. 一樣用加Tab可以嵌套
```

## 超連結
```markdown
* [行內連結](https://www.google.com)
* [帶標題的行內連結](https://www.google.com "Google WebSite")
* [參考連結][Google Link]
[Google Link]: https://www.google.com
```

## 影片

```
[![video test](Video/video.png)](Video/test.mp4)
```

[![video test](Video/video.png)](Video/test.mp4)

## 圖片
```markdown
行內格式：
![圖片文字](01.png "圖片Alt")

參考連結格式：
![圖片文字][logo]
[logo]: 01.png "圖片Alt"
```


## 程式代碼與語法高亮
* 單行代碼用一個`前後包起來
* 多行代碼用三個`前後包起來
* 語法高亮在`符號後加入語法的名稱

<pre><code>
```csharp
Console.WriteLine("Hello");
```
</code></pre>

## 表格
```markdown
冒號用來對齊的
預設為靠左對齊
放在右邊就是靠右對齊
左右都放就是靠中對齊

| 欄位一        | 欄位二           |  欄位三 |
| ------------- |-------------:| :-----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

表示中要跳脫表格用到的符號，需要用html編碼的方式表示
空白是&nbsp;
|是&#124;
```