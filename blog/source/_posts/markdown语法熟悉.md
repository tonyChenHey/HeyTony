---
title: markdown语法熟悉
date: 2022-09-16 17:05:35
tags:
---
### 基本语法

>如果实在忘记了一些语法，用html格式也是可以的噢

#### 标题
用 ***#*** 表示需要写的标题，打多少个表示多少级标题，比如一个表示 **h1** ，两个表示 **h2**，举个例子（三级标题）：  
```
    ### 三级标题
```

#### 换行
可以使用 `<br>` 来表示换行，或者以**两个**或**多个空格**结束后敲**Enter** 来表示换行

#### 加粗
在文字的前后加上`**`就可以了，这么**写**:
```
    为了赚到**钱**，他放下了**面子**
```
#### 斜体
在文字的前后加上`*`就可以了,这么*写*：
```
    *陈小真*是一个人造精神体
```
#### 同时粗体和斜体
在文字前后加上`***`就可以了，这么***写***：

#### 块引用
`>`后接引用的文字，也可以空白用来分段：
```
>单独块引用

>多个段落引用
>
>另一段
```

#### 块嵌套
>块引用中嵌段块引用
> >被嵌套的块
>快引用中嵌套列表  
> - 列表1
> - 列表2  

```
>块引用中嵌段块引用
> >被嵌套的块
>快引用中嵌套列表  
> - 列表1
> - 列表2  
```

#### 有序列表
1. 有序列表用`1. `表示，数字+点+空格；   
3. 前面数字随意，显示出来的里列表都是按顺序的数字的；  
    1. 列表层级注意缩进;     
    3. 缩进的*层级*

```
1. 有序列表用`1. `表示，数字+点+空格；   
3. 前面数字随意，显示出来的里列表都是按顺序的数字的；  
    1. 列表层级注意缩进;     
    3. 缩进的*层级* 
```

#### 无序列表
- 无序列表用`- `表示;
* 也可以用`* `;
+ 还可以用`+ `;
    - 同样层级嵌套注意下缩进  

```
- 无序列表用`- `表示;
* 也可以用`* `;
+ 还可以用`+ `;
    - 同样层级嵌套注意下缩进 
```
#### 列表中添加元素
在列表的中间插入元素，该元素保持一个制表符的缩进就可以了  
- **段落**  
    插入一个段落
* **块引用**  
    >插入一个块引用  
+ **代码块**  
    ```
    consoe.log('hello word!');
    ```
```
- **段落**  
    插入一个段落
* **块引用**  
    >插入一个块引用  
+ **代码块**  
    ```
    consoe.log('hello word!');
    ```
```
#### 代码  
写入`` ` ` ``内，如果要转义显示出 *`* ，类似写脚本中单双引号，用两个``来嵌套
```
    `代码内容`
    ``代码内容需要显示`引用` ``
``` 
#### 代码块
代码块使用两行 **```** ,中间打代码
```
    ```
    中间为代码内容
    ```
```
#### 水平线  
单独一行有多于3个以上的`*`或者`_`或者`-`即可
********************   
_______________________
--------------------------------

```
********************   
_______________________
--------------------------------
```

#### 链接  
`[]`内为链接的文本内容，后面立即接上`()`，将链接打入括号内。

本篇内容参考来源自Markdown中文网中的[文档](http://markdown.p2hp.com/basic-syntax/#overview)
```
本篇内容参考来源自Markdown中文网中的[文档](http://markdown.p2hp.com/basic-syntax/#overview)
```  

- 给链接文本快速加上链接使用`<>`将链接括起来  
    <http://markdown.p2hp.com/basic-syntax/#overview>  
    <chen.chuhai@qq.com>  
    ```
    <http://markdown.p2hp.com/basic-syntax/#overview>
    <chen.chuhai@qq.com>
    ```  
- 格式化链接  
    - 加粗链接  
    **[Markdown文档](http://markdown.p2hp.com/basic-syntax/#overview)**
        ```
        **[Markdown文档](http://markdown.p2hp.com/basic-syntax/#overview)** 
        ```  
    - 格式化带有链接的文本  
        1.首先格式化链接地址部分改为`[]`，其内的链接用一个标签代替，标签不区分大小写，可以包含字母，数字，标点符号，如  
        [Markdown文档][doc]  
        [Markdown文档部分-链接][doc-link] 
        ```   
        [Markdown文档][doc]  
        [Markdown文档部分-链接][doc-link]  
        ```
        2.被格式化的链接标签指向一个实际链接，可以放置在页面任何位置，书写格式有多种： 

        [doc]: http://markdown.p2hp.com/basic-syntax/#overview  
        [doc-link]: http://markdown.p2hp.com/basic-syntax/#links "文档-链接"  

        ``` 
        [doc]: http://markdown.p2hp.com/basic-syntax/#overview  
        [doc-link]: http://markdown.p2hp.com/basic-syntax/#links "文档-链接"  
        ...
        //还有更多写法可以查看文档

        ```  

#### 图片
- 图片  
    图片的书写格式为 **`![图片名称](图片路径)`** ，大概是这样：
    ![引用的图片](https://d33wubrfki0l68.cloudfront.net/eab45e25bb79970178fab7a2d10cba0209372a59/94d9e/assets/images/philly-magic-garden.jpg)  
    ```
    ![引用的图片](https://d33wubrfki0l68.cloudfront.net/eab45e25bb79970178fab7a2d10cba0209372a59/94d9e/assets/images/philly-magic-garden.jpg)  
    ```  
- 图片链接  
    图片链接参考链接添加的方式,在`[]()`的中括号中,按上面图片的图片格式填入图片,后面括号中再填入链接的地址即可。
    [![引用的图片](https://d33wubrfki0l68.cloudfront.net/70a143fdf134aacde3740662a2a47a2a1ee0d216/276c9/assets/images/shiprock.jpg)](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)  
    ```
    [![引用的图片](https://d33wubrfki0l68.cloudfront.net/70a143fdf134aacde3740662a2a47a2a1ee0d216/276c9/assets/images/shiprock.jpg)](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)  
    ```

#### 转义字符  
`\`转义字符  同js的转义，适用于需要用到markdown语法中出现的特殊符号，如\\,\`,\#,\*,\-....
