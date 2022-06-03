# EzUpdate

目录 :

[TOC]

> ---------------------------------------

# 介绍

​        本 模块 以 易语言 所编译，不依赖第三方支持库。

​        本模块不遵循开源协议即不开源，严禁他人对模块进行：反编译、二次贩卖！

# 命令总览

## Bool EzUpdate_Init ( < FileString >  ConfigFile)

***备注***

初始化模块，仅能初始化一次！

若需要再次修改详见 EzUpdate_UnInit 命令

***参数***

< FileString >  ConfigFile  **配置文件路径**  *详见 [ConfigFile](## ConfigFile)*

## Void EzUpdate_UnInit ()

<div id="VoidEzUpdate_UnInit"> </div>

***备注***

可以在 EzUpdate_UnInit () 后再次使用 EzUpdate_Init 实现重新加载配置文件

## Bool EzUpdate_Check ( < Struc_UpdateINFO > OutputInfo )

***备注***

返回 **真** 则有新更新，否则没有

***参数***

< Struc_UpdateINFO > OutputInfo **获取到的配置信息** *详见 [Struc_UpdateINFO](## Struc_UpdateINFO)*

# 文件配置以及结构格式

## ConfigFile

``` Json
{
    "t": "Titile",
    "s": "SubTitle",
    "e": "Text",
    "d": "DownLoadUrl",
    "v": "Version"
}
```

## Struc_UpdateINFO ##

``` EasyLanguage
.版本 2

.数据类型 Struc_UpdateINFO, 公开
    .成员 title, 文本型
    .成员 subtitle, 文本型
    .成员 text, 文本型
    .成员 downloadurl, 文本型
    .成员 version, 文本型
```

# Dev开发记录

## EzUpdate.1.1.1.220531_dev

> 刚开始的第一个开发版本 功能未集全

***Add***

> ***Command***

1. EzUpdate_Init () < 初始化 >
2. Ez_Update_ImportUpdateConfig () < 载入配置文件 >
3. EzUpdate_Check () < 检查 >

> ***GlobalValue***

1. g_cError < 错误信息 >

## EzUpdate.1.2.1.220602_dev

> 进度 + 1

***Add***

> ***Command***

1. EzUpdate_GetInfo () < 在调用 EzUpdate_Check () 之后获取更新信息 >

> ***Structure***

1. Struc_UpdateINFO < 数据结构 >

## EzUpdate.1.2.2.220603_dev

> +1

***Add***

> ***Command***

1. EzUpdate_GetLastError () < 返回 g_cError 信息 >
