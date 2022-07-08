# *ReadME*

<a href="#"><img src="https://img.shields.io/badge/Version-Re--1.0.1.220708--beta-brightgreen"></img></a>   <a href="https://github.com/Qianshi-OriStudio/EzUpdate/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/Qianshi-OriStudio/EzUpdate"></a>   <a href="https://github.com/Qianshi-OriStudio/EzUpdate/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/Qianshi-OriStudio/EzUpdate"></a>   <a href="https://github.com/Qianshi-OriStudio/EzUpdate/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/Qianshi-OriStudio/EzUpdate"></a>   <a href="https://github.com/Qianshi-OriStudio/EzUpdate/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/Qianshi-OriStudio/EzUpdate"></a>  

<a href="https://space.bilibili.com/439946965"><img src="https://img.shields.io/badge/bilibili-ContactMe-pink" alt="与我联系"></img></a>

[toc]

------

## about

| about EzUpdate                                               |
| :----------------------------------------------------------- |
| 你好，开发者。很荣幸能使用此 第三方库 ，此库已重构一次，使代码结构更加清晰明了也让库变得更加易用上手。\n本库还属于 测试版本 ，若您能发现其中里的 bug 或者一些使用上的问题，都可以在 issues 中反馈 :D。 |
| Hello, developer. Thanks for using this Library .The Library is reconstruct  once time *(sorry, my English is so bad. )*, so that, it makes CodeStructure to be the easiest. Now, Version of the Library is still in *Beta* ,if you find some bugs or problem for using, you can feedback on Github-issues :D. |

 ## Public Functions List

| Function     | ReturnType | Paramters                   | About  |
| ------------ | ---------- | --------------------------- | ------ |
| EuInitialize | Bool       | ConfigData \< JsonString \> | 初始化 |

*For Example*

```easyProgramLanguage
EuInitialize (json)
```

Watch Out: json <- stringData is:

``` json
{
    "ApplicationName": "Name",
    "updateType": "Type",
    "urlPath": "GetUrl",
    "ProcAddress": "\<Address\>"
}
```

---

| Function       | ReturnType | About    |
| -------------- | ---------- | -------- |
| EuIsNewVersion | Bool       | 是否最新 |

*For Example*