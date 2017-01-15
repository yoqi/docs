# qrcode介绍

项目地址：http:\/\/tools.yoqi.me\/qrcode\/

（1）qrcode顾名思义就是生成二维码工具。界面如下：

![](/assets/BaiduHi_2017-1-15_12-36-43.png)

（2）qrcode还提供api接口：

http:\/\/tools.yoqi.me\/qrcode\/encode.php?content=

## Req

POST `/api/user/signup`

### Body

| Name        | Type   | Desc   |
|:------------|:-------|:-------|
| mobile      | string | 手机号 |
| pwd         | string | 密码   |
| code        | string | 验证码 |
| couponcode  | string | 送优惠券的兑换码 |
| referrer    | string | 销售来源 可为空, 4位字符串|

```js
{
  "mobile":"18600000000",
  "pwd": "boo",
  "code": "123456",
  "couponcode" : "XWSALES001",
  "referrer" : "1234"

}
```

## Res
### Body
```js
{
  "access_token": "1:+AABOCGhQ8uZTtNqa5uNbYtICCE8zPJp",
  "refresh_token": "1:tESymptHpXXPImUl0gp7DNAPItwu87iJ",
  "token_type": "Bearer",
  "expires_in": 3599
}
```
