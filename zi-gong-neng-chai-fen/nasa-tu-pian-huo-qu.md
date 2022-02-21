---
description: That's one small step for me, one giant leap for mankind.
---

# NASA图片获取

{% embed url="https://github.com/Nambers/NASAForMirai" %}
项目地址
{% endembed %}

{% embed url="https://github.com/Nambers" %}
作者
{% endembed %}

## 可用的指令:

#### #APOD

当天或者指定时间的天文照片

返回转发信息, 里面有照片等其他信息

参数:

* date: 拍摄日期, 以 yyyy-MM-dd格式

#### #EARTH

地球一部分表面照片(和地图的卫星图片差不多), 调用的是google的api所以可能无法使用(建议直接禁用)

返回单张照片

参数:

* lon: 经度
* lat: 纬度
* date: 拍摄日期, yyyy-MM-dd

#### #EPIC

地球全部的照片

返回转发信息里面包含图片和其他信息

目前只支持 [natural/date](https://api.nasa.gov/index.html#:\~:text=natural%20color%20imagery.-,natural/date,-YYYY%2DMM%2DDD)

参数:

* date: 拍摄时间, yyyy-MM-dd

#### #MARS

火星车拍的照片, 有些早的可能发不出

返回转发信息里面包含图片和其他信息

参数：

* earth\_date: 拍摄时间, yyyy-MM-dd
* \<camera>: 可选, 相机名字 FHAZ, RHAZ, MAST, CHEMCAM, MAHLI, MARDI, NAVCAM, PANCAM, MINITES, [对应含义](https://api.nasa.gov/index.html#:\~:text=named%20as%20follows%3A-,Rover%20Cameras,-Abbreviation)
