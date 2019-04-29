[![Latest Stable Version](https://poser.pugx.org/niaoyoo/iplocation/v/stable)](https://packagist.org/packages/niaoyoo/iplocation)
[![Total Downloads](https://poser.pugx.org/niaoyoo/iplocation/downloads)](https://packagist.org/packages/niaoyoo/iplocation)
[![Latest Unstable Version](https://poser.pugx.org/niaoyoo/iplocation/v/unstable)](https://packagist.org/packages/niaoyoo/iplocation)
[![License](https://poser.pugx.org/niaoyoo/iplocation/license)](https://packagist.org/packages/niaoyoo/iplocation)
## 安装

安装这个扩展的首选方式是通过 [composer](http://getcomposer.org/download/).

执行

```bash
composer require niaoyoo/iplocation
```

或添加

```
"niaoyoo/iplocation": "~1.0.0"
```

## 根据IP查询
```php
use IpLocation;

$ipLocation = new IpLocation();
$locationModel = $ipLocation->getLocation('8.8.8.8');
print_r($locationModel);
// Array
// (
//     [ip] => 8.8.8.8
//     [begin_ip] => 8.8.8.8
//     [end_ip] => 8.8.8.8
//     [country] => 美国
//     [area] => 加利福尼亚州圣克拉拉县山景市谷歌公司DNS服务器
// )
```
