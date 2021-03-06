<p align="center">
<a href="https://www.duxravel.com/">
    <img src="https://github.com/duxphp/duxravel/blob/main/resources/image/watermark.png?raw=true" width="100" height="100">
</a>

<p align="center">Duxravel 会员中心</p>

<p align="center">
<a href="https://doc.duxravel.com">中文文档</a>
</p>

<p align="center">
    <a href="https://packagist.org/packages/duxphp/duxravel-member">
        <img src="https://img.shields.io/github/v/release/duxphp/duxravel-member">
    </a>
    <a href="https://packagist.org/packages/duxphp/duxravel-member">
        <img src="https://img.shields.io/packagist/dt/duxphp/duxravel-member.svg?style=flat-square">
    </a>
    <a href="https://packagist.org/packages/duxphp/member">
        <img src="https://img.shields.io/packagist/l/duxphp/duxravel-member.svg?maxAge=2592000&&style=flat-square" alt="Packagist">
    </a>
</p>


## 应用安装
```
// 正式版
composer require duxphp/duxravel-member

// 开发版
composer require duxphp/duxravel-member dev-main
```


## 接口授权
请求登录接口后回去 token 在 header 头中的 Authorization 参数带入授权 token 可请求需授权接口
```
// apifox 请求示例
headers.upsert({
  key: 'Authorization',
  value: 'Bearer ' + token,
});
```

## 接口说明
```
/**
 * 用户登录
 * @params string tel 手机号码
 * @params string password 登录密码
 */
post api/auth/login

/**
 * 用户信息 （授权）
 */
post api/auth/info
```

## 更新日志
```
暂无
```

## 维护者

[@duxphp](https://github.com/duxphp)

## 使用许可

[MIT](LICENSE) © Richard Littauer