# My medicine
A app of Ios or Android
## what is do?
This app allows you to use medication records. You can mark your medication storage locations and dates of validity, etc.
And you can look what medication you have when you go out or have no time to find them.
## the data struction
>### App Data
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
## Main funcation

### ADD
In main window
```txt
[take photo]->OCR->Data
[user inprt]->Data
Data->medication profile
```

