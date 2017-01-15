# qrcode介绍

项目地址：[http://tools.yoqi.me/qrcode/](http://tools.yoqi.me/qrcode/)

（1）qrcode顾名思义就是生成二维码工具。再输入框输入字符，点击确定就会生成关于字符的二维码了。界面如下：

![](/assets/BaiduHi_2017-1-15_12-36-43.png)

（2）qrcode还提供api接口，通过发送给字符请求，返回二维码图片数据：

[http://tools.yoqi.me//qrcode/encode.php/encode.php?content=](http://tools.yoqi.me//qrcode/encode.php/encode.php?content=)

## Req

POST/GET `/qrcode/encode.php`

### Body

| Name | Type | Desc |
| :--- | :--- | :--- |
| content | string | 二维码内容 |

```js
{
  "content":"hello"
}
```

## Res

### Body

```code
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHQAAAB0AQMAAABuVIRkAAAABlBMVEX///8AAABVwtN+AAAAlElEQVQ4jeWSwQ3DMAwDtYH235IbsKSAJG1/op8hgtjHh2BJrHq9SKKIORLWHwQwt4QFqjdHyqwz7hPWZ+O7vw17kNLPfDds9d9ON6w6RFsZw3FoWc98VtzVvsuqiEm9ZOplXFSaShspZDyWJhLy7NN097NjB0m9NFN2nFyvD1iPujIVsbtByLbaoczY83QxdMav1geb9CVDZUVQxQAAAABJRU5ErkJggg==
```



