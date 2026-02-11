# 我的药
iOS 或 Android 的应用
## 做什么？
这个应用允许你使用药物记录。你可以标记药物存放地点和有效期等。
你可以在外出或没时间找药时看看你有的药。
## 数据的破坏
>### 应用数据
>```txt
>Data[
>   users[
>    <user's name>.json
>   ]
>   medication[
>    <user's uuid>.json
>   ]
>]
>```
>```json
>// The users profile
>{
>    "Name": string,
>    "UUID": UUID,
>}
>// The medication profile
>{
>    "Plase01":{
>        "Name":{
>            "0":{
>                "date"{
>                    "y":int,
>                    "m":int,
>                    "d":int
>                }
>                "Note":string,
>            }
>        }
>    },
>    "Plase02":{...},
>    "Plase03":{...},
>    "...":{}
>}
>```
## 主要功能

### ADD
主窗口
```txt
[take photo]->OCR->Data
[user inprt]->Data
Data->medication profile
```

